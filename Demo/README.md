# Machine Problem 1: Demo Early Warning Tool

## Project Overview
This repository contains the deliverables for Machine Problem 1 / Asynchronous Activity 1. The project demonstrates a machine learning workflow built in the KNIME Analytics Platform to train and evaluate a classification model.

## Workflow Files
* **Workflow Archive:** `DemoEarlyWarningTool.knwf`
* **Evidence:** A PDF containing screenshots of the completed step-by-step process is included in the `Demo` folder.

## Algorithms Used
* **Decision Tree Classifier:** The workflow utilizes a Decision Tree Learner node to build the classification model from the training data, and a Decision Tree Predictor node to apply the model to the testing partition.
* **Performance Scoring:** A Scorer node is used to evaluate the accuracy and generate a confusion matrix for the model's predictions.

## Dataset
The dataset required to run this workflow is included in the root of this `Demo` repository folder. 

## Instructions for Running the Workflow
To successfully run this project on your local machine, please follow these steps:

1. **Download the Repository:** Clone or download this GitHub repository to your local machine and extract the files.
2. **Import the Workflow:** 
   * Open the KNIME Analytics Platform.
   * Go to `File` > `Import KNIME Workflow...`
   * Under "Select archive file", browse and select the `DemoEarlyWarningTool.knwf` file from your downloaded folder, then click Finish.
3. **Configure the Data Source:**
   * Open the imported workflow.
   * Locate the **CSV Reader** (or Excel Reader) node at the beginning of the workflow.
   * Right-click the node and select **Configure**.
   * Update the file path to point to the dataset included in this repository's `Demo` folder, then click Apply/OK.
4. **Execute:** 
   * Click the "Execute All Executable Nodes" button (or press `Shift + F7`) to run the pipeline.
   * Right-click the **Scorer** node and select "View: Confusion Matrix" to see the final algorithm results.