---
title: "Smart Traffic Lights (Knowledge Engineering Project)"
collection: portfolio
permalink: /portfolio/smart-traffic-lights
excerpt: "An AI-powered system that optimizes traffic flow by using a Prolog knowledge base, A* search, and HMMs for traffic prediction."
order: 4
date: 2023-06-01 
repo_url: 'https://github.com/bralani/icon22-23'
---

## Goal
Developed for the university's Knowledge Engineering course, this project aims to create an intelligent system to manage traffic intersections. The primary goal is to optimize traffic flow and find the most efficient travel routes by leveraging AI techniques.

## Key Features
- **Prolog Knowledge Base**: The system builds a knowledge base from **OpenStreetMap (OSM) XML** files, representing roads, intersections, and traffic rules in Prolog.
- **Optimal Pathfinding**: It implements the **A* search algorithm** to calculate the most efficient path between two user-specified intersections, providing an estimated travel time.
- **Traffic Prediction**: Utilizes **Hidden Markov Models (HMMs)** to forecast traffic conditions and flow.
- **Semaphore Synchronization**: Includes a feature to globally synchronize traffic lights, aiming to reduce the overall red-light time across the entire monitored area.
- **User Interface**: Provides a menu-driven command-line interface that allows users to load map data, visualize roads and intersections, and request optimal routes.

## Key Metrics & Results
- **Traffic Prediction Accuracy**: The system's HMM-based model achieved an **85% accuracy** in traffic prediction.

## Tech Stack
- Python, Prolog, Pandas, NumPy, Matplotlib, Scikit-learn