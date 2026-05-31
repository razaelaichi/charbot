# Bigram Character Model Report

## A small character model built in a notebook

**By Raza Abbas R H Rizvi - 2026**

## Overview

This project builds a small character model from a list of words. I looked at letter pairs to see which letters follow others, then turned those counts into chances. I also trained a tiny neural network to learn the same idea and watched the loss change during training.

## Project goal

The goal was to learn how a model can pick the next letter in a word. I kept it simple on purpose so I could understand each step.

## How it works in simple terms

- Each word is a chain of letters.
- I add a start mark at the front and an end mark at the end.
- For every pair of letters, I count how often one follows the other.
- I turn those counts into chances by dividing by the total in each row.
- To make new words, I start at the start mark and keep picking the next letter by chance until I hit the end mark.

## What I did

- Loaded a word list and cleaned it into a simple list of words.
- Mapped each letter to a number so it is easy to work with.
- Built a table of letter pair counts.
- Turned the count table into a chance table.
- Sampled new words to see if the model makes sense.
- Built training pairs so the model sees input and the correct next letter.
- Used one hot vectors so the model can read the inputs.
- Trained a small model by adjusting weights and tracking loss.

## What I learned

### Text can become numbers

When you map letters to numbers, you can do math on text. That makes it possible to train a model.

### Counts can become chances

If you count how often one letter follows another, you can turn that into a chance table and use it to guess the next letter.

### Sampling helps you test fast

Sampling is a quick way to see if the model is learning real patterns instead of random noise.

### Training changes the model over time

The weights start with no idea. After many small updates, the model starts to make better guesses and the loss goes down.

## What I saw

- The model could produce short word like outputs.
- The loss numbers moved in a better direction as training went on.

## Key takeaway

Building a small model by hand made the core ideas clear: how text becomes numbers, how chances are built, and how training improves guesses.
