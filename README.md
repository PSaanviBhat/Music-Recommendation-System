# Music Recommendation System

A K-Nearest Neighbors based music recommendation system that suggests songs based on artist and genre similarity using cosine similarity metrics.

## Overview

This project implements an instance-based learning system (K-NN) to recommend songs from a queue of 10 songs. It uses one-hot encoded features for artists and genres, calculates a centroid vector, and finds the most similar songs using cosine similarity.

## Features

- Interactive menu-driven interface
- Dynamic queue management (add/remove songs)
- Real-time recommendations based on current queue
- Search functionality for songs
- Multiple preset queues (Pop, Rock, Mixed)
- Detailed mathematical analysis of recommendations
- Random queue generation for testing

## Tech Stack

- Python 3.8+
- NumPy - Vector operations and matrix computations
- Pandas - Dataset manipulation
- SciPy - Cosine similarity calculations
- Jupyter Notebook

## Dataset

- 100 songs across 30 artists
- 15 genre categories
- Binary one-hot encoding for features
- Format: `Song_Name, Artist_*, Genre_*`

## Installation

```bash
pip install pandas numpy scipy jupyter

```
## Menu Options
1. Add song to queue
2. Remove song from queue
3. View queue and recommendations
4. Clear entire queue
5. View all available songs
6. Search for a song
7. View detailed analysis
8. Create random queue
9. Load preset queue
0. Exit

## Algorithm
The recommendation system works in 4 steps:

- Extract Features: Each song is a binary feature vector
- Calculate Centroid: Mean vector of all songs in queue
- Compute Similarity: Cosine similarity between centroid and all songs
- Rank & Recommend: Return top K most similar songs

## Mathematical Formula
```
Centroid = (v₁ + v₂ + ... + vₙ) / n
Similarity(A, B) = (A · B) / (||A|| × ||B||)
```

## Key Features
1. Fully dynamic - works with any dataset following the structure
2. Real-time recommendation updates
3. Comprehensive error handling
4. Edge case management (empty queue, duplicates, etc.)

## Limitations
- Cold start problem (needs initial queue)
- Equal feature weighting
- Binary encoding may not capture nuanced similarities
- No user history or temporal context

## Future Improvements
- Weighted feature importance
- Audio feature analysis (tempo, key, energy)
- Collaborative filtering
- Deep learning embeddings
- Context-aware recommendations

## How Production Systems Differ
Modern systems (Spotify, Apple Music) use:

- Deep learning and neural networks
- Collaborative filtering with millions of users
- Audio signal processing
- NLP for lyrics analysis
- Reinforcement learning for engagement
- Real-time processing at scale

## Academic Context
This project demonstrates:

- Instance-based learning (K-NN)
- Linear algebra concepts (vectors, centroids, similarity)
- Python scientific computing (NumPy, Pandas, SciPy)
- Software engineering principles

## License
Academic coursework - All rights reserved for educational purposes.

Author
P Saanvi 

Note: This is a rudimentary implementation for educational purposes to understand the mathematical foundations of recommendation systems.