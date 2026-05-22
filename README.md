# UAV Trajectory Optimization for Time-Limited Data Collection in LTE/5G Networks

## About AERPAW

The Advanced Wireless Research Platform (AERPAW) is a National Science Foundation (NSF) research testbed that enables experimentation with UAVs, wireless communications, edge computing, and autonomous systems. This project was developed as part of the AERPAW Autonomous Data Mule (AADM) Challenge, where a UAV collects data from multiple LTE/5G base stations within a constrained mission time.

## Problem Statement

In the AADM challenge, a UAV must maximize the amount of data collected from multiple base stations while satisfying operational constraints such as:

- Limited mission duration
- Geofence restrictions
- UAV mobility constraints
- Dynamic wireless channel conditions

The objective is to maximize the AADM score by efficiently planning the UAV trajectory and selecting the most beneficial base station connections throughout the mission. (https://aerpaw.org/aerpaw-aadm-challenge/)

## Our Approach

We developed an optimization-based framework that jointly considers UAV trajectory planning and base station selection.

Key components include:

- **Adaptive Trajectory Optimization:** The UAV evaluates different visiting orders of base station locations and selects the trajectory that maximizes the final score.
- **MILP-Based Base Station Selection:** For each candidate trajectory, a Mixed Integer Linear Program (MILP) determines the optimal base station association at every time step.
- **Adaptive Speed Control:** The UAV slows down near high-value locations to improve data collection opportunities.
- **Demand-Aware Evaluation:** The framework was evaluated under multiple data-demand distributions, including uniform, exponential, and random scenarios.

Simulation results demonstrated consistent improvements over fixed-trajectory baselines, achieving higher AADM scores and more efficient data collection in dynamic LTE/5G environments.

## Technologies

- MATLAB
- LTE/5G Network Simulation
- Mixed Integer Linear Programming (MILP)
- Gurobi Optimizer
- AERPAW Digital Twin

## Reference

Project report: *UAV Trajectory Optimization for Time-Limited Data Collection in Dynamic Wireless Environments*.
