# Delivery Dispatch Optimization (Main Branch)

This project simulates a package delivery dispatch system using graph-based routing algorithms. It demonstrates how route optimization can help efficiently assign delivery vehicles to customer orders. 

## Purpose 
The `main` branch serves as the base setup of the application.It contains:
- Core project structure.
- CSV files for the delivery network, vehicles, and orders.
- `main.py` to load and verify data.
- An overview of the system.

## Features
- Shortest path delivery routing.
- Load delivery orders and trucks from CSV files.
- Assign orders based on distance and truck capacity.
- Includes negative edge weights to simulate returned packages.

## Dataset Overview
This project uses a realistic delivery network of 50 addresses and 100 delivery orders.

The dataset includes:
- A weighted graph with distances and traffic delays
- Occasional **negative edge weights** to simulate returns or rerouting (e.g., refund trips, misdeliveries)

These features are designed to test both algorithm performance and correctness under real-world conditions.

## Files in This Branch 
- `main.py`: Entry point for testing data loading and structure.
- `delivery_network.csv`: Graph representation of delivery routes. 
- `delivery_prders.csv`: List of delivery destinations and time constraints. 
- `delivery_vehicles.csv`: List of delivery vehicles and their start locations.

## Algorithm Implementstions 
- `dijkstra_branch`: Implements Dijkstra's algorithm for delivery routing. 
- `bellman_ford_branch`: Implements Bellman-Ford algorithm.

## Branch Purpose 
Each branch contains its own test results and timing evaluations. 

## Screenshots 

## Timing Metrics 





