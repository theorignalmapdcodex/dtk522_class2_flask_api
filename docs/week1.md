# Week 1 - Introduction to Design Technology: Bits to Atoms

# MacBook Development Environment Setup Guide

## 1. Installing Anaconda

1. Visit the [Anaconda download page](https://www.anaconda.com/download)
2. Download the macOS installer (choose Apple M1 if you have an M1/M2 Mac, or Windows installer (64-Bit))
3. Open the downloaded .pkg (or .exe) file and follow the installation wizard
4. Verify installation by opening Terminal and running:

```bash
conda --version
```
2. Setting up Git

Install Homebrew (if not already installed):

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Install Git using Homebrew:

```bash
brew install git
```

Configure Git with your credentials:

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

Verify installation:

```bash
git --version
```

3. Installing Required Python Packages

Create a new conda environment (optional but recommended):

```bash
conda create -n myenv python=3.10
conda activate myenv
```

Install packages using pip:

```bash
pip install streamlit openai anthropic chromadb flask
```

4. Installing a Text Editor
Option 1: VS Code

Visit the VS Code download page
Download and install the macOS version
Install recommended extensions:

Python
Pylance

Option 2: Cursor

Visit the Cursor download page
Download and install the macOS version
Follow the setup wizard to configure AI features

Verifying Everything Works

Open Terminal and check Python environment:

```bash
python --version
```

Verify package installation:

```bash
pip list
```

Test Git:

```bash
mkdir test-project
cd test-project
git init
```

Test Python environment with a simple script:

```python
# Create a test.py file in your editor
import streamlit as st
import openai
import anthropic
import chromadb
from flask import Flask

print("All packages imported successfully!")
```

Run the script:

```bash
python test.py
```

