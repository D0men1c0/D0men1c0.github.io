---
title: "VisionAI Assistant (LauzHack 2024)"
collection: portfolio
permalink: /portfolio/visionai-lauzhack
excerpt: "A multi-modal AI assistant developed in 22 hours at EPFL, capable of analyzing images using natural language voice commands."
date: 2024-12-30
repo_url: 'https://github.com/D0men1c0/LauzHack'
---

## Goal
Developed in just 22 hours for the LauzHack hackathon at EPFL, VisionAI Assistant is a functional prototype of a mobile application that can analyze and interpret visual content using complex natural language queries, delivered via text or voice.

## Technical Architecture & Workflow
The system employs a sophisticated multi-modal architecture to process user requests:
1.  **Input & Transcription**: User provides a voice or text query. Voice commands are transcribed to text using **Whisper**.
2.  **Query Understanding**: The text query is processed by **SBERT** to identify the primary object of interest (e.g., "cars").
3.  **Image Segmentation**: Meta's **Segment Anything Model (SAM 2)** receives the image and the object class from SBERT, segmenting all relevant objects and outputting their bounding boxes.
4.  **Feature Engineering**: A structured dataset is created from the bounding boxes, enriching it with engineered features like **color, size, and position** for each segment.
5.  **LLM-Powered Filtering**: **GPT-4o** receives the full natural language query and the structured dataset. It dynamically writes and executes code to filter this dataset based on the user's specific constraints (e.g., "red cars", "in the center").
6.  **Output**: The application visually highlights the filtered bounding boxes on the original image and returns the answer.

## Key Features
- **Complex, Multi-Attribute Queries**: Unlike standard VLMs, users can ask complex questions filtering by object type, color, size, and location (e.g., "How many red cars are on the left?").
- **Multi-Modal Interaction**: Accepts input via both text and voice for maximum flexibility.
- **Modular & Scalable Design**: The backend, built with **Flask** and hosted on **AWS EC2**, separates NLP, CV, and filtering tasks, making the system maintainable and scalable.
- **Dynamic Code Generation**: Leverages GPT-4o not just for understanding, but for actively writing filtering code, enabling high precision on engineered features.

## Tech Stack
- **Frontend**: Flutter
- **Backend**: Flask, AWS EC2
- **AI Models**: Whisper, SBERT, Segment Anything Model (SAM 2), GPT-4o