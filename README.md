# Micro-Ecosystem Simulation

This project simulates a micro-ecosystem with predators and prey to explore basic concepts in evolutionary biology using genetic algorithms. The simulation aims to model predator-prey interactions and observe how traits evolve over generations to improve survival and reproduction within an environment.

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [How It Works](#how-it-works)
- [Future Enhancements](#future-enhancements)
- [Contributors](#contributors)

## Project Overview

This simulation is designed to help study predator-prey dynamics and basic evolutionary principles. It features two main agent types, **Prey** and **Predator**, with distinct behaviors. Each agent has traits represented as genes, which determine its ability to survive, hunt, and evade within a 2D grid environment. Over generations, these traits evolve using a genetic algorithm, simulating natural selection and mutation.

## Features

- **Agent-Based Modeling**: Prey and predator agents move around a 2D grid, interacting based on defined behaviors.
- **Genetic Algorithm**: Traits evolve across generations, with selection, mutation, and crossover steps to simulate evolution.
- **Energy Mechanics**: Agents expend energy while moving; predators gain energy by catching prey.
- **Visual Representation**: Simple 2D visualization of the ecosystem using PyGame.
- **Configurable Parameters**: Easily modify traits, population sizes, and genetic algorithm parameters.

## Requirements

- **Python 3.x**
- **NumPy**
- **PyGame** (for visualization)
- **DEAP** (for the genetic algorithm components)

To install dependencies, use:
"pip install numpy pygame deap"

## Installation

- **Clone the Repo:**
    git clone https://github.com/yourusername/micro-ecosystem-simulation.git
- **Install Required Dependencies:**
    pip install -r requirements.txt

## Usage

**1.** Run the simulation by executing the following command:
    python simulation.py

**2.** A window will open showing the 2D grid with prey (green) and predators (red) moving around. Observe how they interact and evolve over time.

## How It Works

- **Agents:** Prey and Predator classes inherit from a base Agent class, each initialized with traits like speed, energy, and movement patterns. Prey move randomly to avoid predators, while Predators hunt based on proximity to prey.

- **Genetic Algorithms:** Implemented using the DEAP library, where each agent's traits are treated as a genome.
Fitness scores are assigned based on survival and reproduction success, guiding selection, crossover, and mutation in each generation.

- **Energy Mechanism:** Prey gain energy by consuming food, while predators gain energy by consuming prey.
Each movement action decreases energy, and agents with zero energy are removed from the environment.

- **Visualisation:** A basic PyGame window shows real-time interactions between prey and predators. Green circles represent prey; red circles represent predators.

## Future Enhancements
- **Adaptive Behaviors:** Introduce more complex behaviors like group movement or hiding.
- **Trait Inheritance:** Track which traits lead to higher survival and reproduction rates across generations.
- **Resource Distribution:** Add more complex environmental factors, such as varying food sources and obstacles.
- **Data Visualization:** Plot population dynamics over time to observe evolutionary trends.

## Contributors
- Vatsal Labh (vatsalla@buffalo.edu)
- SaeHan Jang (saehanja@buffalo.edu)
- Gregory Kojemiako (gkojemia@buffalo.edu)
- Milton Morris (morris56@buffalo.edu)