# Podcast-to-Book Recommendation System

A dual-agent NLP system that leverages podcast preferences to recommend books, demonstrating how agentic AI can provide personalized, context-aware content recommendations.

## Overview

This system combines semantic understanding and user modeling to bridge the gap between podcast listening preferences and book recommendations. By analyzing podcast descriptions, the system infers user interests and matches them with relevant books using advanced embedding techniques.

## Architecture

### Dual-Agent System
- **Profiler Agent**: Analyzes podcast descriptions to extract user interests and personality traits using keyword extraction and sentence embeddings
- **Recommender Agent**: Compares user interest vectors with precomputed book embeddings using cosine similarity to suggest relevant and diverse books

## Technical Implementation

### Embedding Models
The system evaluates two sentence embedding models:

| Model | Pros | Cons | Use Case |
|-------|------|------|----------|
| all-MiniLM-L6-v2 | Lightweight, fast computation | Lower semantic precision | Quick prototyping |
| all-mpnet-base-v2 | Deep contextual understanding, higher accuracy | More computational overhead | Production recommendations |

**Performance Results:**
- MPNet: 40%+ average relevance score
- MiniLM: ~30% average relevance score

### Similarity Scoring
- **Metric**: Cosine similarity between user interest vectors and book embeddings
- **Score Range**: 30-95%
- **Categories**: Low, Medium, High relevance tiers for interpretable filtering

### Visualization
Interactive Plotly charts compare embedding model performance, highlighting MPNet's superior semantic matching capabilities.

## Key Features

- Real-time podcast description analysis
- Semantic book matching
- Multi-tier relevance scoring
- Interactive performance visualizations
- Comparative model evaluation
