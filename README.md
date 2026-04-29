# Data-Driven Game System in Python

A console-based game system built on top of dynamically collected data, combining web scraping, data processing, and interactive gameplay.

## Overview

This project demonstrates how external data can be transformed into a functional system. It consists of two main components:

1. **Data Pipeline** – extracts and structures data from external sources  
2. **Game Engine** – uses that data to drive game logic and player interaction  

---

## Architecture

### 1. Data Pipeline (`data_pipeline.py`)

- Scrapes Pokémon data from an external website
- Extracts:
  - Name
  - Types
  - Attack moves and power
- Transforms raw HTML into structured Python objects
- Splits data into:
  - Current attacks
  - Future attacks (progression system)
- Serializes data into JSON (`pokemons.json`)

Key concepts:
- Web scraping
- Data extraction & cleaning
- Structured data modeling
- Serialization (JSON)

---

### 2. Game Engine (`game_engine.py`)

- Loads structured data from JSON into Python objects
- Simulates a turn-based combat system
- Manages player state:
  - Team composition
  - Inventory (pokeballs, potions)
  - Captured Pokémon
- Implements game mechanics:
  - Combat system (attack / defend loop)
  - Health management
  - Experience and leveling system
  - Move learning and progression
  - Probabilistic capture system

Key concepts:
- State management
- Object-oriented design
- Game loop architecture
- System interaction (files, persistence)

---

## Data Flow

1. Scrape raw data from web
2. Transform into structured format
3. Store locally (JSON)
4. Load into objects
5. Use as input for game logic

---

## Example Features

- Dynamic Pokémon generation from real data
- Turn-based combat system with user input
- Experience and leveling mechanics
- Move replacement system on level-up
- Capture system based on enemy health probability
- Persistent storage of captured Pokémon

---

## Technologies

- Python
- requests-html (web scraping)
- JSON (data persistence)
- Object-Oriented Programming

---

## Purpose

This project was built to explore:

- Data-driven system design  
- Transforming unstructured data into usable systems  
- Connecting data pipelines with application logic  
- Managing complexity in interactive programs  

---

## What I Learned

- Designing systems that separate data processing from execution logic  
- Working with real-world, unstructured data sources  
- Structuring and persisting data for later use  
- Building interactive systems with state and progression  

---

## Potential Improvements

- Fix edge cases (e.g., negative inventory values)  
- Prevent duplicated Pokémon objects in team  
- Improve capture system logic and balancing  
- Add modularization and testing  
- Introduce a proper database (SQLite)  
