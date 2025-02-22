# Boen-PS2: Twitter Bot Detection Analysis

This repository contains code and data for analyzing Twitter bot detection using a sampled subset of the **Twibot-22** dataset. The dataset is originally introduced in:

> Feng, Shangbin, Zhaoxuan Tan, Herun Wan, Ningnan Wang, Zilong Chen, Binchi Zhang, Qinghua Zheng et al.  
> "Twibot-22: Towards graph-based Twitter bot detection."  
> *Advances in Neural Information Processing Systems*, 35 (2022): 35254-35269.

Due to the large size of Twibot-22, this project includes a **sample of 1,000 users** while preserving key user attributes, social connections, and bot/human labels.

## Hardware Requirements

### Minimum Configuration:
- **CPU**: Intel i5 or Apple M1 (MacBook Pro M1)
- **RAM**: 8 GB
- **Disk Space**: 50 GB (for dataset storage and computations)
- **OS**: macOS, Ubuntu 20.04, or Windows 10

### Recommended Configuration:
- **CPU**: Intel i7 or Apple M1 Pro/Max (for improved performance)
- **RAM**: 16 GB+
- **Disk Space**: 100 GB (for large-scale experiments)
- **OS**: macOS, Ubuntu 20.04, or Windows 10

## Software Requirements

- **Operating System**: macOS (Apple M1/M2 chip), Ubuntu 20.04, or Windows 10  
- **Programming Language**: Python 3.8+  

# ⚙️ Setup Instructions

## 1️⃣ Local Setup

### 1. Clone the Repository
Open a terminal and run:


```python
from google.colab import drive
drive.mount('/content/drive')

%cd /content/drive/MyDrive/Boen-PS1/code

import os
os.system('jupyter nbconvert --to notebook --execute EDA.ipynb')



```bash
git clone https://github.com/Rising-Stars-by-Sunshine/Boen-ps2.git
cd Boen-ps2
cd code
