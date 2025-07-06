# Delivery Route Optimization (Dijkstra Branch)

This branch implements Dijkstra’s Algorithm for route optimization in a simulated package delivery system.

## Purpose

To demonstrate shortest path routing using the Dijkstra algorithm in a delivery context. This branch runs independently of the main and Bellman-Ford branches.

## Features
- Implements Dijkstra’s Algorithm for shortest path routing
- Loads delivery network, orders, and trucks from CSV files
- Assigns delivery orders based on travel time and availability
- Measures algorithm runtime in milliseconds
- `Note`: Dijkstra's algorithm assumes all edge weights are non-negative.  
  The algorithm may miss shorter paths or produce suboptimal results because it does not account for reductions in total cost.

## Files in This Branch
- `dijkstra.py`: Implements the core Dijkstra algorithm
- `main.py`: Runs the simulation and timing test
- CSV Files:
    - `delivery_network.csv`
    - `delivery_orders.csv`
    - `delivery_vehicles.csv`

## Algorithm Used

**Dijkstra’s Algorithm**  
A greedy algorithm that finds the shortest path from a starting point to all other nodes in a weighted graph with non-negative edge weights.

## Timing Test

## Output Screenshot

*Include a screenshot here once tests are complete*

## Branching Strategy

This branch is **not merged** with `main` or `bellman_ford_branch`. Each branch remains isolated for clean testing and comparison of routing algorithms.