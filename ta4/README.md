# ta4_formoso.py - AI Reasoning Systems Demonstration

This repository contains `ta4_formoso.py`, a simple Python script that demonstrates foundational Artificial Intelligence reasoning techniques using a basic computer troubleshooting scenario.

## Features

The script is divided into three main components:

1. **Knowledge Representation**: 
   - Uses a dictionary-based knowledge base to store current system facts (e.g., `wont_turn_on`, `beep_codes`) and categories (e.g., `power`, `display`)[cite: 1].
2. **Rule-Based Reasoning (RBR)**[cite: 1]:
   - Features a basic inference engine that runs through predefined rules (`rule_power`, `rule_ram`, `rule_screen`)[cite: 1].
   - Outputs specific troubleshooting actions based on the current facts[cite: 1].
3. **Case-Based Reasoning (CBR)**[cite: 1]:
   - **Retrieve**: Calculates similarity scores between a new problem and a database of past cases[cite: 1].
   - **Reuse**: Suggests the solution from the best matching past case[cite: 1].
   - **Revise**: Interactively prompts the user to confirm if the solution worked, allowing for manual revision if it failed[cite: 1].
   - **Retain**: Adds the new problem and its final (or revised) solution to the case base for future use[cite: 1].

## Prerequisites

- Python 3.x[cite: 1]

## How to Run

1. Clone or download the script to your local machine.
2. Open a terminal or command prompt.
3. Run the script using the following command:

```bash
python ta4_formoso.py