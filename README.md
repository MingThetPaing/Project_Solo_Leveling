# Project_Solo_Leveling

**Table of Contents**
- [About the Project](#about-the-project)
- [Features](#features)
- [How to run the code](#how-to-run-the-code)
- [How to play? (expected input and output)](#how-to-play-expected-input-and-output)
- [Data Structure Used](#data-structure-used)

## About the Project
Problem Statement: Nowadays, people tend to procrastinate and cannot follow regular to do lists or goals.  
Objective: Inspired by the anime "Solo Leveling", this project aims to gamify the person's self improvement journey by giving their todolist as missions and earning XPs as rewards to level up.  
This project works for many goals. As an example, I used weight loss to demonstrate.

## Features
- **Adaptive Mission Generation**:  
  Missions scale in difficulty based on total XP:  
  - Easy : Low-reward missions (e.g., "Run 3 km")  
  - Medium : Mid-reward missions (e.g., "Run 5 km")  
  - Hard: High-reward missions (e.g., "Run 7 km")  

- **Mission Types**: 
  - Strength: Push-ups, sit-ups  
  - Stamina: Running  
  - Willpower: Diet (calories deficit, protein)  

- **Mission Tracking**: 
  - Pending Missions: Stored in a deque (FIFO queue)  
  - Resets missions at the start of a new day

## How to run the code
Using python, the code is very easy to run on Google Colab, Jupyter Notebook or Vscode. After running the code, you are qualified to be "The Player".

## How to Play (expected input and output)
- After running the code, the player will be asked to accept the challenge (Y/N)
- After pressing Y:  
  The game officially begins  
  - New players start at Level 1  
  - Returning players load progress from progress.json  

- **Game Menu** to choose from:  
  1. Complete next mission: Marks the top mission as done (grants XP)  
  2. Start new day: Refresh missions  
  3. Exit: Saves progress and quits  

- **Progress**:  
  - Missions auto-scale in difficulty based on your XP  
  - Unlock more difficult missions by earning more XP  
  - Level up when respective XP reaches 100  
  - Ensure to click enter between each action!

## Data Structure used
- **Queue (deque)**: Tracks missions to be completed in FIFO order  
- **Lists**: 
  - Current available missions  
- **Dictionaries**:
  - Tracks XP per category levels  
  - Skill levels per category  
- **Json** is also used to track progress
