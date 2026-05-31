# Bigram Character Model

## A small notebook project

This is a simple learning project that builds a small character model from a list of words. It counts letter pairs, turns them into chances, and samples new words. It also trains a tiny neural network to predict the next letter.

## Why this project

I wanted to understand the basics of how text models work. I kept it small so each step is easy to follow.

## What it does

- Reads a word list and prepares it for training.
- Counts which letters follow others.
- Turns counts into chances and samples new words.
- Trains a small model to predict the next letter.

## How to run

1. Open the notebook in this repo in Jupyter or VS Code.
2. Make sure Python and PyTorch are installed. Example: `pip install torch`
3. Run the cells from top to bottom.

## What you will see

- A table of letter pair counts.
- Sample words produced by the model.
- Loss values that change during training.

## What I learned

- How to turn letters into numbers a model can use.
- How counts can become chances.
- How a simple loss and weight update can improve guesses.

## Notes

This project is small and made for learning. It is a good base to grow into bigger models later.
