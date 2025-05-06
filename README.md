# RNN_LSTM_TRANSFORMER
# RNN_LSTM_TRANSFORMER: Character-Level Language Modeling on *Alice in Wonderland*

This project implements and compares three different neural network architectures—**SimpleRNN**, **GRU**, and **Transformer**—for a character-level language modeling task. The goal is to predict the next character in a sequence using a recurrent or attention-based model.

## 📚 Dataset

We use the *Alice in Wonderland* text, a classic and publicly available work of literature, making it ideal for exploring language modeling. The dataset is preprocessed into sequences of fixed length (e.g., 40 characters) to be fed into the models for training.

## 🧠 Models Implemented

### 1. SimpleRNN
A basic recurrent neural network that learns from character sequences by maintaining a hidden state. Due to its simplicity, it struggles with long-term dependencies and often results in repetitive or grammatically incorrect outputs.

### 2. GRU (Gated Recurrent Unit)
An advanced RNN variant that includes gating mechanisms to retain long-term dependencies. This model significantly outperformed SimpleRNN in both training loss and output quality.

### 3. Transformer
A lightweight transformer-based model using self-attention to model long-range dependencies more efficiently. Despite its shallow depth, it showed promise in stylistic output and fast convergence.

## ⚙️ Training Setup

- **Framework**: TensorFlow / Keras
- **Sequence length**: 40 characters
- **Batch size**: 64
- **Embedding size**: 128
- **Hidden size**: 256 (for RNN/GRU)
- **Epochs**: 20 (adjustable in notebook)
- **Loss Function**: Sparse Categorical Crossentropy
- **Optimizer**: Adam
- **Environment**: Google Colab and local machine with GPU support

## 📈 Results

| Model        | Final Training Loss | Output Quality               |
|--------------|---------------------|------------------------------|
| SimpleRNN    | ~1.3                | Repetitive, less coherent    |
| GRU          | ~1.0                | Most coherent and fluent     |
| Transformer  | ~1.5                | Stylistic, but fragmented    |

## 📝 Example Outputs

### SimpleRNN:

### GRU:

### Transformer:


## 🎯 Conclusion

The **GRU model** provided the best balance between efficient training and coherent text generation, thanks to its ability to retain contextual information. The **Transformer** showed high potential with faster convergence but underperformed slightly due to model depth and dataset size. The **SimpleRNN** served as a useful baseline, highlighting the limitations of basic recurrent units.

## 📎 Files

- `RNN_NLP.ipynb`: Jupyter notebook with all model code, training loops, and generation examples
- `README.md`: Project summary and documentation
- `training_loss_plot.png`: Visual comparison of loss curves



## 👨‍🎓 Author

Zach Wilson – AI Final Exam, Spring 2025  
Oklahoma State University, Graduate Program in Electrical & Computer Engineering

