# Delivery Route Optimization (Bellman-Ford Branch)

This branch implements the Bellman-Ford Algorithm for route optimization in a simulated delivery system.

## Algorithm Used
- **Bellman-Ford Algorithm**: A dynamic programming algorithm that finds the shortest paths even when negative weights are present (not typical in delivery networks, but useful for learning and comparison).

## Dataset Used 
The delivery network includes a small percentage of **negative distances** to simulate situations such as:
- Returned packages
- Wrong delivery corrections
- Cost-adjusted rerouting

This tests Bellman-Ford's correctness, as Dijkstra’s algorithm would not work properly with such data.
## Functionality
- Loads graph data from `delivery_network.csv`
- Dispatches vehicles from `delivery_vehicles.csv`
- Assigns each order based on the shortest path calculated by Bellman-Ford
- Measures and prints path, cost, and execution time

## Features
- Implements Bellman-Ford Algorithm for route optimization
- Supports negative edge weights for experimentation
- Loads input data from CSV files
- Includes performance timing and path output
- Handles graphs with **negative edge weights**.
- Can correctly compute routes involving refunds, returns, or priority reroutes.

## Files in This Branch
- `bellman_ford.py`: Core Bellman-Ford implementation
- `main.py`: Simulation runner and timing tracker
- CSV Files:
  - `delivery_network.csv`
  - `delivery_orders.csv`
  - `delivery_vehicles.csv`

## Timing Test