# McKinsey Solve Ecosystem Building Game - Solution

This repository contains my solution to the McKinsey Solve Ecosystem Building mini-game. The challenge involves selecting 8 species from a list of 39 to build an ecosystem that meets several key objectives. The game simulates real-world ecosystem dynamics, and this solution follows a structured approach to tackle the game’s complexities.

## Game Overview

In the Ecosystem Building mini-game, you are tasked with building a sustainable ecosystem with 8 species that meets three objectives:

1. **Form a Continuous Food Chain**: Each species in the ecosystem must connect to others through a valid predator-prey relationship.
   
2. **Calorie Surplus**: Every predator-prey pair must have a calorie surplus, ensuring that prey provides more energy than predators consume.
   
3. **Terrain Specifications**: Each species must match the terrain requirements of the chosen location. You will be working in either the Mountain or Reef environment.

## Solution Breakdown

### Objective 1: Terrain Match

The two terrain scenarios, Mountain and Reef, have specific terrain parameters such as temperature, elevation, and depth. The species you choose must have terrain requirements that match those of the selected location. 

- **Mountain Terrain Specifications**: Includes parameters like elevation, temperature, wind speed, and precipitation.
- **Reef Terrain Specifications**: Includes water-related parameters such as depth, current speed, and salt content.

### Objective 2: Food Chain Continuity

Each species in the game is categorized into producers (plants/corals) or consumers (herbivores, carnivores, omnivores). The food chain needs to start with producers and end with apex predators, with each link in the chain ensuring a sustainable calorie flow.

- **Producers**: Provide energy from natural elements (e.g., sunlight).
- **Consumers**: Must have valid prey and predator relationships. Apex predators have no natural predators and consume energy from the top of the chain.

### Objective 3: Energy Balance

The calorie balance is vital for the ecosystem to survive. Each species has its own caloric needs (Calories Needed) and production (Calories Provided). The goal is to ensure:

- **Predators** have enough prey to satisfy their caloric needs.
- **Prey** species are not consumed to extinction by ensuring a caloric surplus.

The game applies specific "eating rules" to simulate how species consume prey and interact with their environment, which is modeled in this solution.

## Solution Approach

### Step 1: Select the Location
Start by analyzing the terrain specifications for the selected environment (Mountain or Reef). The terrain specs are the most crucial step in deciding which species can survive in the ecosystem. A spreadsheet or scratch paper can help to map out the terrain specifications and identify species that are compatible.

### Step 2: Build the Food Chain
After selecting the environment, the food chain is built using either a top-down or bottom-up approach:

- **Top-down approach**: Start by selecting an apex predator with low caloric needs and build downwards by adding prey that meets its caloric requirements.
- **Bottom-up approach**: Start by selecting producers with high caloric output and build upwards by adding predators.

The solution ensures that every species in the food chain has both adequate calories and a valid predator-prey relationship.

### Step 3: Triple-check and Adjust
Once the food chain is built, verify that all species meet the terrain specifications, have sufficient caloric intake, and are not driven to extinction by over-consumption. Adjust the chain if necessary.

## Key Challenges

1. **Terrain Match Complexity**: Different species have complex terrain requirements, which must align with the selected environment.
   
2. **Caloric Balancing**: Maintaining a caloric surplus for each species is critical. The solution must ensure predators do not over-consume prey species to extinction.
   
3. **Data Processing**: The game provides a large volume of data for each species. Efficient organization and processing of this data is essential to success.

## Solution Files

- **`McKinseyGame_vf.ipynb`**: The Jupyter notebook containing my full solution to the McKinsey Solve Ecosystem Building mini-game. It walks through the problem, terrain analysis, food chain building, and caloric balancing in detail.

## How to Run the Solution

1. **Install Requirements**: Ensure that Python and Jupyter are installed on your machine. The notebook requires basic libraries such as `numpy`, `pandas`, and `matplotlib`.
   
2. **Open the Notebook**: Launch the `McKinseyGame_vf.ipynb` notebook in Jupyter and follow along with the analysis and solution steps.

## Conclusion

This solution provides a systematic approach to tackling the McKinsey Solve Ecosystem Building mini-game. By focusing on terrain compatibility, food chain continuity, and caloric balance, the solution ensures a sustainable and functional ecosystem.
