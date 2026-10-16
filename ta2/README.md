# Rule-Based Vacuum Agent

This project is a small Python simulation of a vacuum-cleaning agent. The agent checks the room where it is located, cleans the room if it is dirty, and moves to the other room if the current room is already clean.

## Project purpose

The program demonstrates a simple rule-based intelligent agent:

1. The agent observes the current room.
2. If the room is dirty, it cleans the room.
3. If the room is clean, it moves to the other room.
4. The process repeats for the number of steps selected by the user.

The environment has two rooms: Room A and Room B. The agent always starts in Room A.

## Requirements

- Python 3.7 or later

No external libraries are required.

## How to run

1. Save `ta2_formoso.py` and `README.md` in the same folder.
2. Open a terminal in that folder.
3. Run:

   ```bash
   python ta2_formoso.py
   ```

   On some systems, use:

   ```bash
   python3 ta2_formoso.py
   ```

The program also runs in Google Colab by uploading the Python file or pasting the code into a cell and running the cell.

## User input

When prompted, enter:

- `dirty` or `clean` for Room A
- `dirty` or `clean` for Room B
- A whole number for the number of simulation steps

Example inputs:

```text
Room A state: dirty
Room B state: clean
How many steps should the simulation run? 4
```

## Example behavior

If Room A is dirty, the first action is to clean Room A. If Room A is clean, the agent moves to Room B. On the next step, it applies the same rules to its new location.

The program displays the agent's location, the action it takes, and the current state of both rooms after every step.

## Main components

- `rooms`: A dictionary that stores the state of Room A and Room B.
- `is_dirty()`: Checks whether a room's state is `dirty`.
- `clean_room()`: Changes a room's state to `clean`.
- `VacuumAgent`: Stores the agent's location and defines its movement and decision-making behavior.
- Simulation loop: Repeats the agent's actions based on the number of steps entered by the user.

## Limitations

This is a basic rule-based simulation. It only has two rooms, the agent can move between them, and it does not validate incorrect room states or non-numeric step inputs.
