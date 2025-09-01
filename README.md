This project aims to build a dual-agent NLP system that recommends books based on a user's preferred podcasts, exploring the intersection of recommendation systems and agentic AI.\
The Profiler Agent analyzes podcast descriptions to infer user interests and personality traits using keyword extraction and sentence embeddings.\
The Recommender Agent compares the user’s interest vector with precomputed book embeddings using cosine similarity to suggest relevant and diverse books.\
The system showcases how agent-based architectures can provide personalized, context-aware content recommendations by integrating semantic understanding and user modeling.\

Embedding Model Comparison \
● The system evaluates two prominent sentence embedding models—all-MiniLM-L6-v2 and all-mpnet-base-v2—to balance computational efficiency with semantic accuracy. \
● While MiniLM is lightweight and offers faster computation, it falls short in delivering precise semantic matches, making it less effective for nuanced recommendations. \
● On the other hand, MPNet provides deeper contextual understanding and higher average relevance scores, making it more suitable for content-rich domains like books and podcasts. \

Similarity Metric: Cosine Similarity \
● Cosine similarity is the core metric used to assess the alignment between a user’s interest vector (generated from podcast descriptions) and the semantic embeddings of books. \
● It computes the cosine of the angle between two vectors, effectively capturing the degree of thematic similarity between user preferences and book content. \
● Cosine similarity scores range from 30% to 95%, with results categorized into low, medium, and high relevance tiers to facilitate interpretability and recommendation filtering. \

Evaluation Visualization \
● The comparative performance of the two embedding models is visualized using Plotly, showcasing their respective average relevance scores through a bar chart.\
● The chart highlights that all-mpnet-base-v2 achieves an average relevance score exceeding 40%, while all-MiniLM-L6-v2 remains in the low 30% range. Deployment and Accessibility \

