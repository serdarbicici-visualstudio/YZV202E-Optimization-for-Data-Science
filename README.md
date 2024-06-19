# Optimizing ISPARK Parking Lot Management in Istanbul

## Authors
- **Batuhan Sal**
  
- **Omer Erdağ**
  
- **Serdar Biçici**


## Project Overview
This project utilizes a genetic algorithm to optimize the assignment of cars to parking lots in Istanbul, aiming to improve parking efficiency and user satisfaction while reducing costs and environmental impact.

## Problem Description
The main challenge is to assign each car to an optimal parking lot considering various parameters like distance, gas cost, budget, and parking fees. Traditional approaches focusing solely on the nearest parking lot often lead to overcrowding and inefficiency.

## Methodology
- **Data Collection and Preprocessing**: Retrieved parking lot data from the ISPARK API, processed and filtered relevant information.
- **Class Design**:
  - **Park Class**: Manages parking lot attributes and operations.
  - **Car Class**: Handles car attributes such as location, gas usage, and parking duration.
- **Genetic Algorithm**: Includes functions for creating an initial population, selection, crossover, mutation, and fitness evaluation. The algorithm iteratively improves car-to-parking lot assignments based on fitness scores.

## Fitness Functions
Two fitness functions were used to evaluate the optimization:
- **Reverse Linear**: Focuses on minimizing total costs, including gas and parking costs, and maximizing space utilization and user satisfaction.
- **Linear**: Similar approach with different weightings for cost, space utilization, and user satisfaction.

## Experiments and Results
Various experiments were conducted to assess the impact of population size, mutation rate, generation number, and different fitness functions on the optimization process. Key findings include:
- Larger populations and higher mutation rates generally improve fitness scores.
- Excessive generations yield diminishing returns.
- The linear fitness function performed slightly better in terms of distance and cost metrics.

## Conclusion
The genetic algorithm outperformed the traditional nearest-parking strategy by considering multiple parameters and avoiding overcrowded parking lots. This approach leads to reduced emissions, lower costs for users, and more efficient use of parking resources, demonstrating its potential for improving urban parking management.
