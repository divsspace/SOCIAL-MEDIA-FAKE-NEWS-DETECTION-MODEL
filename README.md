# SOCIAL-MEDIA-FAKE-NEWS-DETECTION-MODEL

# Abstract
This project leverages Graph-Based Neural Networks (GNNs) for analysing social media data to extract meaningful insights such as community detection, fake news detection, sentiment propagation, and influencer identification. By modelling social media interactions as graphs—where nodes represent users or posts and edges represent relationships such as retweets, mentions, and likes—graph neural networks can uncover patterns that are challenging for traditional machine learning models to detect.
We focus on fake news detection using a Relational Graph Convolutional Network (R-GCN) trained on the ACL 2017 Rumor Detection Dataset from Twitter (twitter15 and twitter16). The dataset, available on Kaggle, provides labeled tweets categorized as true, false, unverified, or non-rumor. Our approach involves constructing a graph using tweet interactions and computing text-based features (TF-IDF, sentiment analysis), which are then enhanced with semantic and statistical features. These graphs are fed into the R-GCN model to learn node representations, enabling the prediction of misinformation. The goal is to develop a robust and scalable system for social media analysis that can be extended to other tasks, including influencer detection and sentiment analysis.

System Architecture
1. Input: Twitter datasets (twitter15 and twitter16) with labelled tweets.
2. Graph Representation: Nodes represent tweets, and edges represent relationships based on cosine similarity of text features.
3. Model: R-GCN with two graph convolutional layers, skip connections, and dropout for stability.
4. Output: Class predictions for each tweet (true, false, unverified, non-rumor).

Dataset
• Dataset Name: ACL 2017 Rumor Detection Dataset (Twitter15 & Twitter16)
• Source: Kaggle
• Labels: True, False, Unverified, Non-rumor

