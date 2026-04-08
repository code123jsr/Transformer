# Transformer Implementation from Scratch

## Introduction
This project implements a **Transformer model from scratch** for both text classification and language modeling tasks. The code includes encoder, decoder, and advanced variations, with training loops, tokenization, and utilities to visualize attention maps. The models achieve strong results in **accuracy** (for classification) and **perplexity** (for language modeling).

## Project Highlights
- Implemented a Transformer encoder and decoder from scratch.
- Achieved high classification accuracy on text datasets.
- Achieved low perplexity in language modeling tasks on speeches datasets (Obama, H. Bush, W. Bush).
- Experimented with advanced techniques like **ALiBi positional encoding** and **disentangled multi-head attention** to optimize model performance.

## File Structure
- `transformer.py`: Contains encoder, decoder, and other Transformer modules.  
- `main.py`: Training loops, dataset loading, and script to run all experiments.  
- `utilities.py`: Utilities class for sanity checks and attention map visualization.  
- `tokenizer.py`: `SimpleTokenizer` class for building vocabulary and encoding/decoding text.  
- `dataset.py`: Dataset classes for text classification and language modeling.  
- `speechesdataset/`: Folder containing required text and TSV files for training.  

## Usage
In `main.py`, there are three options: `part1`, `part2`, and `part3`. Enter the required option to run a specific experiment.

### Part 1: Encoder (Classifier Training)
- Train a classifier using the Transformer encoder.  
- Prints **loss and test accuracy** for every epoch.  
- Provides a sanity check and **attention map visualization** for a sample sentence.  

### Part 2: Decoder (Language Modeling)
- Train a Transformer decoder for language modeling.  
- Prints **training perplexity** every 100 iterations on training and test sets (Obama, H. Bush, W. Bush).  
- Provides a sanity check and **attention map visualization** for a sample sentence.  

### Part 3: Model Exploration for Improvement
- Experiment with advanced architectures and hyperparameters.  
- Techniques include **ALiBi positional encoding**, **disentangled multi-head attention**, and other improvements.  
- Prints **loss and test accuracy** during training for selected models.  

## Results
- High classification accuracy on the provided dataset.  
- Low perplexity on language modeling tasks.  
- Advanced architectural experiments improved both performance and stability.
