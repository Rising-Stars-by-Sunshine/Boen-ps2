# Code Folder

## 1. Overview
This folder contains Jupyter Notebooks for analyzing **Twitter Bot Detection**, **Social Network Analysis**, and **Causal Inference**. The tasks include performing social network analysis using centrality measures, training predictive models using hypergraph neural networks, and applying **Regression Discontinuity Design (RD)** to study the impact of Twitter’s subscription program on user engagement.

## 2. Files Included

- **`causal_inference.ipynb`**: 
  - **Purpose**: Implements Regression Discontinuity Design (RD) to investigate the impact of Twitter’s subscription program on user engagement, such as weekly study time or tweet frequency.
  
- **`Explanation.ipynb`**: 
  - **Purpose**: Performs social network analysis on the **Twibot-22** dataset, focusing on the differences between human and bot accounts in terms of centrality measures, including degree centrality, closeness centrality, and betweenness centrality.

- **`prediction.ipynb`**: 
  - **Purpose**: Trains a **Hypergraph Neural Network** to detect Twitter bots by leveraging user profile features and social network relationships.

## 3. Prerequisites

### Required Libraries and Versions:
- **Python 3.9**
- **networkx==2.5**
- **easygraph==1.4.1**
- **pandas==1.3.2**
- **statsmodels==0.13.2**
- **matplotlib==3.4.3**
- **seaborn==0.11.2**
- **torch==1.9.0**
- **numpy==1.21.1**
- **torch.nn** (included in the `torch` library)
- **sklearn==0.24.2**

### Installation Instructions:

1. Clone the repository:

    ```bash
    git clone https://github.com/Rising-Stars-by-Sunshine/Boen-ps2.git
    cd Boen-ps2
    ```

2. Install dependencies using `pip`:

    ```bash
    pip install -r requirements.txt
    ```

3. To install specific libraries individually, use:

    ```bash
    pip install networkx==2.5 Easygraph==1.4.1 pandas==1.3.2 statsmodels==0.13.2 matplotlib==3.4.3 seaborn==0.11.2 torch==1.9.0 numpy==1.21.1 sklearn==0.24.2
    ```

## 4. Usage Instructions

### Step-by-Step Guide:

1. **Loading Datasets**:
   - Ensure that the dataset files (`user_sample.json`, `label_sample.csv`, `edge_sample.csv`) are in the correct directory.


2. **Running Social Network Analysis**:
   - For social network analysis, run the following notebook to analyze centrality measures and their differences between bots and humans:

    ```bash
    jupyter notebook Explanation.ipynb
    ```

3. **Training and Evaluating Predictive Models**:
   - To train a hypergraph neural network model for bot detection, run the following:

    ```bash
    jupyter notebook prediction.ipynb
    ```

4. **Running Causal Inference Analysis**:
   - To perform Regression Discontinuity Design (RD) analysis on the impact of Twitter’s subscription program, execute:

    ```bash
    jupyter notebook causal_inference.ipynb
    ```

## 5. Expected Outputs

- **Visualizations**: 
  - CDF of centrality measures between human and bot, distirbution of centrality mesuares and plot of training loss of Hypergraph Neural Network(HGNN) .
  
- **Performance Metrics**: 
  - Metrics like accuracy, ROC-AUC for bot detection models.

- **Explanatory Insights**:
  - For causal inference, insights into the causal effects of Twitter’s subscription program on user engagement.

## 6. Contributors

- **Boen Liu** – Project Lead, Branstorming, Causal Inference, Social Network Analysis, Predictive Modeling, Hypergraph Neural Network. 
