# Wind Farm Layout Optimization

## About
This project focuses on optimizing the layout of a wind farm to maximize Annual Energy Production (AEP). Using a penalty-based gradient descent approach, the optimization considers wake effects, wind speed variations, and spatial constraints to ensure efficient turbine placement within a defined area.

---

## Project Objectives
- **Maximizing AEP**: Place turbines in high wind-speed zones to maximize energy production.  
- **Minimizing Wake Losses**: Incorporate wake effect modeling to reduce energy losses due to turbine interactions.  
- **Constraint Adherence**: Ensure turbine placement satisfies boundary conditions and maintains minimum spacing of 400m.  

---

## Approach
1. **Input Data**: The project uses a wind speed map (`wind_speed_map.csv`) as input, representing the spatial distribution of wind speeds over a 4 km x 4 km area.  
2. **Objective Function**: The objective function calculates AEP based on turbine positions, wind speed, and wake losses.  
3. **Optimization Method**:  
   - **Penalty Method**: Introduces penalties for violating constraints like boundary limits and inter-turbine spacing.  
   - **Gradient Descent**: Iteratively adjusts turbine positions to maximize AEP while satisfying constraints.  
4. **Output**: The optimized layout maximizes AEP while adhering to constraints and minimizing wake interference.  

---

## Key Features
- **Data-Driven Layout Optimization**: Relies on a wind speed map for turbine placement decisions.  
- **Wake Effect Modeling**: Implements models to estimate energy losses due to wake interactions.  
- **Constraint Handling**: Ensures all turbines are within the boundaries and maintain adequate spacing.  
- **Visualization Tools**: Provides visual insights into the optimization process and final layout.  

---

## Getting Started

### Prerequisites
- Python 3.8+  
- Required Libraries: NumPy, Matplotlib, Pandas, Scipy  

### Setup
1. Clone the repository:  
   ```bash
   git clone <repository_link>
   cd WindFarmOptimization
   ```
2. Install dependencies:  
   ```bash
   pip install -r requirements.txt
   ```
3. Open the Jupyter Notebook to run and analyze the optimization:  
   ```bash
   jupyter notebook WindFarmOptimization.ipynb
   ```

---

## Usage
1. **Load Wind Speed Map**: Input the wind speed map (`wind_speed_map.csv`) into the provided notebook.  
2. **Configure Parameters**: Adjust algorithm parameters, including learning rate, iterations, and penalty factors.  
3. **Run Optimization**: Execute the notebook to optimize turbine placements.  
4. **Visualize Results**: View the optimized layout and corresponding AEP improvements through heatmaps and charts.

---

## Results
- **Initial Layout**: Turbine positions based on random or uniform placement strategies.  
- **Optimized Layout**: Enhanced turbine positions that maximize AEP while maintaining constraints.  
- **Performance Metrics**: Visualization of AEP improvement and wake loss reduction.

---

## Key Files
- `WindFarmOptimization.ipynb`: Main notebook with the optimization algorithm, visualizations, and analysis.  
- `wind_speed_map.csv`: Input dataset for wind speed distribution over the target area.  
- `report.pdf`: Detailed project documentation, including methodology, results, and insights.  

---

## Future Work
- Extend the optimization to handle dynamic wind conditions.  
- Explore advanced optimization techniques like Genetic Algorithms or Particle Swarm Optimization.  
- Integrate real-world turbine data for validation and scalability.  

---

## Contributing
Contributions are welcome! Fork this repository, make improvements, and submit a pull request.

---

## License
This project is licensed under the MIT License.

