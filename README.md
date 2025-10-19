# capstoneproject
Capstone Project for Data Classification and Summarization Class with Hactiv8 and IBM SkillsBuild

The Scholar's Lens: Translating Unstructured Research Abstracts into Actionable Insights Using IBM Granite
Project Overview
This project, "The Scholar's Lens," is a capstone for the Hacktiv8 X IBM SkillsBuild program. It addresses the challenge of information overload in scientific research, where millions of papers are published annually, making it impossible for professionals to keep up.

The goal is to develop an intelligent tool that leverages the untapped potential of early-access papers from archives like arXiv. Instead of just finding papers, this tool is designed to help users focus, clarify, and interpret complex information.

Objectives
Dual-Classification System: Automatically classify scientific abstracts by both Subject Area and Research Methodology using the IBM Granite model.
Abstractive Summarization: Condense technical abstracts into concise, easy-to-understand summaries.
Visualize Research Trends: Generate visualizations to reveal patterns and leading categories in research.
Synthesize Actionable Insights: Interpret the outputs to formulate strategic recommendations.

Methodology & Tech Stack
Core AI Model: IBM Granite Large Language Model.
Key Technique: Zero-Shot Prompt Engineering for flexible and powerful categorization without traditional model training.
Technical Stack: Google Colab, Python, Pandas, LangChain, Matplotlib, and Seaborn.

The project utilizes the arXiv Paper Abstracts dataset available on Kaggle. This dataset is a large, open-access collection of metadata from scientific papers, primarily focusing on fields like physics, mathematics, computer science, and quantitative biology.
Link: https://www.kaggle.com/datasets/spsayakpaul/arxiv-paper-abstracts 
Dataset Size: 56,181 rows spanning three columns (terms, titles, and abstracts).


The analysis of the dataset revealed several key insights into the current landscape of scientific research.
A word cloud of the most frequent terms shows a research community focused on building and testing new approaches. Words like model, method, propose, neural, and network dominate the vocabulary, painting a clear picture of a field driven by innovation. 

An analysis of two-word phrases confirms that "neural networks" and "deep learning" are central topics. The most frequent phrase, "state art" (state-of-the-art), highlights a highly competitive culture focused on outperforming existing benchmarks.

A heatmap of interdisciplinary research shows strong collaborations between fields like "Machine Learning" and "Statistics ML," demonstrating they are almost inseparable in modern research. It also highlights fields like "Cryptography" that operate in relative isolation.

The analysis also identified the top three most active research categories, with Computer Vision and Machine Learning representing the two largest fields by a significant margin, followed by Statistics - Machine Learning.


The project's intelligent capabilities are powered by two key components:

IBM Granite: This is the Large Language Model (LLM) that performs all the core NLP tasks. It follows complex instructions from prompts to categorize papers by subject and methodology (without prior training on this specific task) and rewrites dense, technical abstracts into structured, easy-to-understand summaries.

Replicate AI: Replicate is a cloud platform that hosts various AI models, including IBM Granite. It provides a simple and standardized API that acts as a bridge, allowing the Python code in Google Colab to send requests to the IBM Granite model and receive the results.
