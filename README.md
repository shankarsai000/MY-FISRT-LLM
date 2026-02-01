🧠 My First LLM (Bigram Model)
This repository documents my journey into understanding Large Language Models (LLMs). This is a simple Character-Level Bigram Language Model built from scratch using PyTorch.

The goal of this project was to demystify how models like GPT work by building the fundamental architecture: the "Next Token Predictor."

📂 What's Inside?
This project takes a raw string of text (Shakespearean style), learns the statistical probability of which character follows another, and generates new text based on those probabilities.

simple_llm.py: The complete code containing the data processing, model architecture, training loop, and generation script.

Architecture: A simple Neural Network using nn.Embedding.

Tokenizer: Character-level tokenization (mapping letters to integers).

🚀 Getting Started
Prerequisites
You need Python installed, along with PyTorch.

Bash
pip install torch
Running the Model
Clone the repo and run the script:

Bash
python simple_llm.py
📊 How it Works
Tokenization: It breaks text down into individual characters.

Training: The model looks at a character (e.g., "T") and adjusts its weights to predict the next character (e.g., "o").

Generation: We give it a starting character, and it samples the next one based on the probabilities it learned.

📝 Sample Output
Note: Since this is a simple Bigram model (it only looks 1 character back), the output resembles English words but lacks deep semantic meaning.

"To be or not to be... forthe st me..." (Example)

📚 Learnings
Building this helped me understand:

How computers process text using Tensors.

The concept of Logits and Softmax.

The basic Training Loop (Forward pass -> Loss -> Backward pass).

Why modern LLMs need Self-Attention (Transformers) to act smarter than this model.

🔜 Next Steps
My plan to upgrade this model:

[ ] Implement a Self-Attention Head.

[ ] Upgrade to a full Transformer Block.

[ ] Train on a larger dataset (like the collected works of Shakespeare).

Built with 🐍 Python and 🔥 PyTorch as part of my AI learning journey.****
