# Drone Simulator Project

## Introduction

This project involves a drone simulator designed to navigate and map an environment using different algorithms. The primary goal is to compare the efficiency of these algorithms in terms of area discovered.


## Project Structure

- **Simulator**: The core simulation environment where the drone navigates through a given map.
- **Algorithms**: Different strategies implemented for the drone to explore the map.
- **Improvements**: Enhancements made to the original simulator and algorithms.

## Improvements Made

### Simulator Enhancements

1. **Battery Consumption Model**: Improved battery consumption model to ensure the drone's battery lasts exactly 8 minutes (480 seconds) under typical usage. The simulator runs until the drone's battery is depleted.
2. **Accurate Area Calculation**: Refined the area calculation method to consider only navigable areas, excluding walls and obstacles.
3. **Enhanced Visualization**: Updated the visualization components to better represent the drone's path and the explored areas.

### Algorithm Enhancements

1. **Optimized Pathfinding**: Improved pathfinding algorithms to ensure more efficient coverage of the map.
2. **Better Decision Making**: Enhanced decision-making logic to reduce redundant movements and improve overall coverage.
3. **Adaptive Speed Control**: Implemented adaptive speed control based on the environment and battery levels.

## Algorithm Comparison

We conducted several tests to compare the performance of different algorithms. The comparison is based on the area discovered by the drone.

### Results Summary

#### Average of 5 Runs on Map 4

| Algorithm          | Area Discovered Average (%) |
|--------------------|-----------------------------|
| Original Algorithm | 45.045%                     |
| Improved Algorithm | 77.362%                     |

#### Single Run Outcomes on Other Maps

| Map   | Algorithm          | Area Discovered (%) |
|-------|--------------------|---------------------|
| Map 1 | Original Algorithm | 68.00%              |
|       | Improved Algorithm | 91.13%              |
| Map 2 | Original Algorithm | 74.6%               |
|       | Improved Algorithm | 100%                |
| Map 3 | Original Algorithm | 57.29%              |
|       | Improved Algorithm | 98.5%               |
| Map 5 | Original Algorithm | 30.72%              |
|       | Improved Algorithm | 82.88%              |


## Visual Comparisons

### Map 2

**Original Algorithm:**

![Original Algorithm - Map 2](Outcomes\Map2\OriginalAlgo\74%.PNG)

**Improved Algorithm:**

![Improved Algorithm - Map 2](Outcomes\Map2\ImprovedAlgo\100%.PNG)

### Map 3

**Original Algorithm:**

![Original Algorithm - Map 3](Outcomes\Map3\OriginalAlgo\57%.PNG)

**Improved Algorithm:**

![Improved Algorithm - Map 3](Outcomes\Map3\ImprovedAlgo\improved(98%).PNG)

### Map 4

**Original Algorithm:**

![Original Algorithm - Map 4](Outcomes\Map4\OriginalAlgo\56%.PNG)

**Improved Algorithm:**

![Improved Algorithm - Map 4](Outcomes\Map4\ImprovedAlgo\88%.PNG)

### Map 5

**Original Algorithm:**

![Original Algorithm - Map 5](Outcomes\Map5\OriginalAlgo\30%.PNG)

**Improved Algorithm:**

![Improved Algorithm - Map 5](Outcomes\Map5\ImprovedAlgo\82%.PNG)

### Discussion

The improvements in the algorithm have led to a significant increase in the area discovered. The improved algorithm consistently outperformed the original algorithm across different maps.

## How to Run the Simulator

1. **Setup**:
    - Clone the repository.
    - Ensure you have the necessary dependencies installed.

2. **Running the Simulator**:
    - Navigate to the project directory.
    - In the "SimulatorWindow" file in line 186 change the current path to the map you want to load without the last number and the ".png" finisher
    - Run the "SimulationWindow" file to start the simulation.

3. **Configuring the Maps**:
    - Maps can be found in the `Maps` directory.
    - Modify the map files or add new ones to test different environments.

## Future Work

1. **Further Optimization**: Continue refining the pathfinding and decision-making algorithms.
2. **Real-World Integration**: Explore the integration of the simulator with real-world drone hardware.
3. **Advanced Visualization**: Enhance the visualization to include 3D representations and real-time analytics.

## Original Project

- You can find the original project that we improved in this link: 
- https://github.com/vection/DroneSimulator

## Contributors

- [Lior Jerbi](https://github.com/LiorJerbi)
- [Yael Rosen](https://github.com/yaelrosen77)
- [Tomer Klugman](https://github.com/tomerklugman)
- [Hadas Evers](https://github.com/hadasevers)
