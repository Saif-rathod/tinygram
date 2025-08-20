# TinyGram 🧠📜
A minimal yet powerful Bigram Language Model implemented from scratch using Python and NumPy. Designed to help you understand the core concepts behind probabilistic language models.

## 🚀 Features
- Pure Python + NumPy implementation
- Bigram probability matrix from corpus
- Sampling-based text generation
- Clean, educational code

---

## 📦 Installation


git clone https://github.com/saif-rathod/tinygram.git
cd tinygram
pip install -r requirements.txt
If you only use NumPy and no external libs, you may skip requirements.txt.

🛠️ Usage
1. Train the Bigram Model
bash
Copy
Edit
python train.py --data data/input.txt
This will:

Tokenize the corpus

Build the bigram count matrix

Normalize into a probability matrix

Save the trained model (optional)

2. Generate Text
bash
Copy
Edit
python generate.py --start_token "T" --length 100
Sample Output:

css
Copy
Edit
The time that the torm tore tore that tom tame the...
📚 Theory Behind
The model uses the Bigram approach, where the probability of the next character/token depends only on the current one:

sql
Copy
Edit
P(w2 | w1) = Count(w1, w2) / Count(w1)
It builds a vocabulary-size x vocabulary-size matrix of probabilities and samples from it to generate new sequences.

✅ Requirements
Python 3.7+

NumPy

🧠 Learn More
The Illustrated Transformer

Speech and Language Processing - Jurafsky & Martin

🤝 Contributing
PRs are welcome! Feel free to fork this repo and improve it:

Add smoothing (e.g., Laplace)

Extend to Trigram/Neural LMs

Use word-level instead of character-level tokens
