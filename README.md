
# Optimizing Solar Site Selection in Turkey using Genetic Algorithms and Particle Swarm Optimization

## Project Overview
This project focuses on identifying the optimal locations for solar energy installations across Turkey by applying **Genetic Algorithms (GA)** and **Particle Swarm Optimization (PSO)**. The goal is to maximize solar potential while ensuring geographic diversity and minimizing proximity to existing solar plants.

## Problem Description
The main objective is to select a fixed number of locations that maximize environmental suitability for solar energy. The suitability is determined by factors such as solar irradiance, clearness index, cloud cover, and precipitation. The challenge includes managing the trade-off between selecting high-suitability sites and avoiding overcrowding or proximity to existing installations.

## Methodology
- **Data Collection and Preprocessing**: 
  - Environmental data (suitability scores) for 733 locations in Turkey.
  - Real-world data of existing solar plants in Turkey.
- **Genetic Algorithm**:
  - Random population initialization.
  - Selection based on fitness, crossover, mutation.
  - Fitness includes suitability scores and penalties for proximity.
- **Particle Swarm Optimization**:
  - Particles represent location combinations.
  - Positions updated based on cognitive and social components with decaying coefficients.
  - Fitness calculated similarly to GA.
- **Visualization**:
  - Heatmaps, scatter plots, and interactive maps generated using Matplotlib and Folium.

## Fitness Function
The fitness function is a weighted sum of environmental suitability factors, penalized by:
- Proximity to other selected points (to avoid clustering).
- Proximity to existing solar plants (to encourage new development areas).

## Experiments and Results
Experiments were conducted to evaluate the impact of population size, mutation rate, iteration count, and different (c1, c2) parameter settings on the optimization results. Key findings include:
- Larger populations and moderate mutation rates improve solution quality.
- PSO decaying parameters help balance exploration and exploitation.
- The optimization methods outperform simple greedy selection by achieving higher overall suitability scores and better spatial distribution.

## Conclusion
Both Genetic Algorithms and Particle Swarm Optimization effectively identify optimal locations for solar energy installations. By considering environmental factors and spatial diversity, the methods contribute to more strategic and sustainable solar energy planning in Turkey.
