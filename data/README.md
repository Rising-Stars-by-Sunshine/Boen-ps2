# Twibot-22 Sample Dataset

This folder contains a subset of the **Twibot-22** dataset, which is a large-scale benchmark for Twitter bot detection. The original dataset, introduced by **Feng et al. (2022)**, provides a comprehensive collection of Twitter user profiles, social connections, and bot/human annotations to facilitate research on bot detection using graph-based and machine learning approaches.

Due to the large size of Twibot-22, this sample includes **1,000 users**, preserving key user attributes, social relationships, and labels. The dataset aims to help researchers experiment with bot detection models without requiring extensive computing resources. The full dataset and its details can be found in the paper:

> Feng, Shangbin, Zhaoxuan Tan, Herun Wan, Ningnan Wang, Zilong Chen, Binchi Zhang, Qinghua Zheng et al.  
> "Twibot-22: Towards graph-based Twitter bot detection."  
> *Advances in Neural Information Processing Systems*, 35 (2022): 35254-35269.

## 📌 Dataset Source and Purpose

- **Source**: The full dataset is available at [Twibot-22 Official Website](https://twibot22.github.io/).
- **Purpose**: This dataset is designed to facilitate research on **Twitter bot detection** by providing a structured, real-world dataset for machine learning and graph-based models. It enables researchers to develop, evaluate, and compare different bot detection methodologies while ensuring scalability for large-scale social network analysis.

## 📂 Files
- **`user_sample.json`** – Contains user profile information.
- **`label_sample.csv`** – Includes bot/human labels for users.
- **`edge_sample.csv`** – Represents relationships between users.

## 📖 Data Dictionary

| File               | Column             | Description |
|--------------------|-------------------|-------------|
| user_sample.json  | created_at         | Account creation date |
|                   | description        | User bio |
|                   | entities           | Embedded links/media info |
|                   | id                 | Unique user ID |
|                   | location           | User location |
|                   | name               | Display name |
|                   | pinned_tweet_id    | Pinned tweet ID |
|                   | profile_image_url  | Profile picture URL |
|                   | protected          | Whether the account is private |
|                   | public_metrics     | Follower, following, tweet count, etc. |
|                   | url                | Profile URL |
|                   | username           | Twitter handle |
|                   | verified           | Verification status |
|                   | withheld           | Withheld regions (if any) |
| edge_sample.csv   | source_id          | Source user ID |
|                   | relation           | Type of relationship (e.g., follow, retweet, quote, post, like) |
|                   | target_id          | Target user ID |
| label_sample.csv  | id                 | User ID (matching user_sample.json) |
|                   | label              | human, bot |

## 🔄 Preprocessing and Harmonization Steps

To ensure data consistency and usability, the following preprocessing steps were applied:

1. **Filtering Users**:  
   - Selected a **balanced subset of 1,000 users**, ensuring diversity in bot/human distribution.
   - Removed inactive or deleted accounts from the original dataset.

2. **Graph Structure Processing**:  
   - Extracted relevant social relationships (e.g., follows, retweets, mentions).
   - Constructed an edge list (`edge_sample.csv`) to facilitate network analysis.

This dataset serves as a basis for evaluating Twitter bot detection models.
