---
title: "VisionAI Assistant (LauzHack 2024)"
collection: hackathons
date: 2024-12-30
venue: "EPFL, Lausanne"
role: "Participant"
excerpt: "A multi-modal AI assistant developed in 22 hours, capable of analyzing images using natural language voice commands."
header:
  image: lauzhack.jpg
  teaser: lauzhack.jpg
repo_url: 'https://github.com/D0men1c0/LauzHack'
---

Developed over an intensive 22-hour period at the LauzHack hackathon at EPFL, VisionAI Assistant is a functional prototype of a multi-modal AI application. The system can interpret complex, natural language voice commands to analyze visual content in images. 

Its architecture uses SBERT to identify objects of interest, Meta's Segment Anything Model (SAM 2) for precise segmentation, and GPT-4o to dynamically generate and execute code for filtering based on multiple attributes like color, size, and position. This allows for sophisticated queries such as "How many red cars are on the left side of the image?".