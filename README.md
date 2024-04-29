# Neural Machine Translation with PyTorch

This project implements a neural machine translation (NMT) system using PyTorch. The goal is to translate text from French to English using a sequence-to-sequence (seq2seq) model with attention mechanism.

## Project Overview

The NMT model consists of an encoder-decoder architecture, where the encoder reads input sequences (French sentences) and converts them into a fixed-size context vector. The decoder then uses this context vector to generate output sequences (English translations).

### Model Components

- **Encoder RNN**: Processes input sequences using a Gated Recurrent Unit (GRU) and produces encoder hidden states.
  
- **Decoder RNN**: Utilizes an attention mechanism (specifically Bahdanau attention) to selectively focus on parts of the input sequence while generating the output sequence.

### Data Preparation

The project uses parallel data from the Tatoeba project, which provides translations of sentences in various languages. The dataset is preprocessed by tokenizing sentences, filtering by length, and normalizing text.

### Requirements

To run this project, ensure you have:
- Python 3.x
- PyTorch
- NumPy

Install the required packages using `pip`:

```bash
pip install torch numpy
