# Hide-And-Seek Game Agent

Hide-And-Seek Game Agent is a Unity 3D project where an NPC uses a Multi-Criteria Decision-Making method to intelligently select hiding spots. The agent evaluates possible hiding locations, chooses the safest option, and moves through the environment while trying to avoid detection by the player.

## Demo

# Gameplay Demo

[![Watch the video](https://img.youtube.com/vi/VH9ivYNfitc/0.jpg)](https://youtu.be/VH9ivYNfitc)

## Tech Stack

- Unity
- C#

### Decision Making

- A* Pathfinding
- Weighted Sum Model
- Multi-Criteria Decision Making
- Raycast-based visibility detection

### Environment

- 3D Unity scene
- 2D grid-based navigation system
- Dynamic hiding spot evaluation

## Features

- Intelligent NPC hiding behavior
- Weighted Sum Model for hiding spot selection
- A* pathfinding for NPC movement
- Dynamic hiding spot re-evaluation
- Player proximity detection
- Real-time raycast visibility check
- Safety score calculation based on player visibility and distance
- Escape route availability evaluation
- Game over condition when the NPC is spotted
- Unity 3D environment with grid-based movement logic

## Requirements

- Unity Hub
- Unity 2022.3.28f1 LTS or newer

## How It Works

The NPC uses a grid-based A* algorithm to move through the environment. Available hiding spots are evaluated using multiple criteria:

- Distance from the player
- Safety score
- Escape route availability

Each criterion is weighted and combined using the Weighted Sum Model. The hiding spot with the highest final score is selected as the NPC's target.

When the player comes within 20 grid tiles of the NPC, the agent re-runs the decision-making process and may switch to a safer hiding location.

## Gameplay demo
[![Watch the video](https://img.youtube.com/vi/VH9ivYNfitc/0.jpg)](https://youtu.be/VH9ivYNfitc)
