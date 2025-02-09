# Wind Farm Layout Optimization

This repository contains the implementation of a wind farm layout optimization algorithm. The goal is to maximize Annual Energy Production (AEP) by optimizing turbine placements based on a wind speed map and considering wake effects. The solution uses a penalty method combined with gradient descent to handle spatial and physical constraints effectively.

Project Objectives
Maximizing AEP: Place turbines in high wind-speed zones to maximize energy production.
Minimizing Wake Losses: Incorporate wake effect modeling to reduce energy losses due to turbine interactions.
Constraint Adherence: Ensure turbine placement satisfies boundary conditions and maintains minimum spacing of 400m.
Approach
Input Data: The project uses a wind speed map (wind_speed_map.csv) as input, representing the spatial distribution of wind speeds over a 4 km x 4 km area.
Objective Function: The objective function calculates AEP based on turbine positions, wind speed, and wake losses.
Optimization Method:
Penalty Method: Introduces penalties for violating constraints like boundary limits and inter-turbine spacing.
Gradient Descent: Iteratively adjusts turbine positions to maximize AEP while satisfying constraints.
Output: The optimized layout maximizes AEP while adhering to constraints and minimizing wake interference.
Key Features
Data-Driven Layout Optimization: Relies on a wind speed map for turbine placement decisions.
Wake Effect Modeling: Implements models to estimate energy losses due to wake interactions.
Constraint Handling: Ensures all turbines are within the boundaries and maintain adequate spacing.
Visualization Tools: Provides visual insights into the optimization process and final layout.
Getting Started
Prerequisites

Python 3.8+
Required Libraries: NumPy, Matplotlib, Pandas, Scipy
