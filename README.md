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

```bash
git clone https://github.com/Rising-Stars-by-Sunshine/Boen-ps2.git
cd Boen-ps2
cd code
```

### 2. Create a Virtual Environment (Recommended)
It is recommended to use a virtual environment to manage dependencies.

#### macOS/Linux:
```bash
python3 -m venv env
source env/bin/activate
```

#### Windows (Command Prompt):
```bash
python -m venv env
env\Scripts\activate
```

### 3. Install Dependencies
Run the following command to install required Python libraries:

```bash
pip install pandas==1.2.4 matplotlib==3.4.3 networkx==2.5 numpy==1.19.2
```

### 4. Verify Installation
Ensure all libraries are correctly installed by running:

```bash
python -c "import pandas, matplotlib, networkx, numpy; print('Setup successful!')"
```

### 5. Run EDA Notebook
Navigate to the `code` directory and run the `EDA.ipynb` Jupyter Notebook.


## 2️⃣ Cloud Setup

For users who want to run the project on cloud platforms like Google Colab or AWS, follow these steps:

### 1. Google Colab Setup

#### 1. Open Colab and Mount Google Drive
Open [Google Colab](https://colab.research.google.com/) and run the following command to mount your Google Drive:

```python
from google.colab import drive
drive.mount('/content/drive')
```

#### 2. Clone the Repository
Navigate to a suitable directory in your Google Drive and clone the repository:

```bash
%cd /content/drive/MyDrive/
git clone https://github.com/Rising-Stars-by-Sunshine/Boen-PS1.git
%cd Boen-PS1/code
```

#### 3. Install Dependencies
Install the required dependencies:

```bash
!pip install pandas==1.2.4 matplotlib==3.4.3 networkx==2.5 numpy==1.19.2
```

#### 4. Run Jupyter Notebook
Run the following command to open `EDA.ipynb` in Colab:

```python
from google.colab import drive
drive.mount('/content/drive')

%cd /content/drive/MyDrive/Boen-PS1/code

import os
os.system('jupyter nbconvert --to notebook --execute EDA.ipynb')


