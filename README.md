# LangChain-OpenAI-API

---

# Installation Guide

Welcome to the installation guide. This document will walk you through the steps to get everything set up and running. 

## Prerequisites

Before you begin, ensure you have Python installed on your machine. This project is built to run with Python, so it's essential.

## Step 1: Install Langchain and Other Required Packages

Langchain, along with several other necessary packages, are required for this project to function correctly. Install them using pip by running the following command in your terminal:

```sh
pip install langchain openai chromadb tiktoken unstructured
```

## Step 2: Configure Your API Key

To use this project, you'll need an OpenAI API key. Follow these steps to configure your environment:

1. Locate the file named `constants.py.default` in the root directory.
2. Open it with your preferred text editor.
3. Replace the placeholder text with your actual OpenAI API key.
4. Save the file and rename it to `constants.py`.

This step is crucial for enabling the communication with OpenAI's services.

## Step 3: Prepare Your Data

You'll need to place your own data into the project for it to read and interact with:

1. Navigate to the `data` directory within the project.
2. Place your text data into a file named `data.txt`.

This file will be used by the project to read and respond to your queries.

# Example Usage

Once installation and configuration are complete, you're ready to test the setup. Here are a couple of examples to get you started:

## Test Reading from Text File

To test reading from the `data/data.txt` file, use the following command:

```sh
python chatgpt.py "what is my dog's name"
```

Expected output:

```
Your dog's name is Sunny.
```

## Test Reading from PDF File

To test reading from a PDF file named `data/cat.pdf`, use this command:

```sh
python chatgpt.py "what is my cat's name"
```

Expected output:

```
Your cat's name is Muffy.
```

