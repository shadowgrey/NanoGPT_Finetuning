# 🧠 Fine-Tuning NanoGPT

This repository contains my fine-tuned version of NanoGPT, a compact yet powerful GPT implementation by Andrej Karpathy. I experimented with various hyperparameter configurations and ultimately settled on the following setup:

block_size: 384  
vocab_size: 50304   # Based on GPT-2's vocab size (50257), padded to the nearest multiple of 64  
n_layer: 8  
n_head: 8  
n_embd: 384   
dropout: 0.0  


As the name suggests, NanoGPT is designed to be a lightweight model. This makes generating logically coherent responses more challenging compared to larger models. To address this, I explored multiple hyperparameter combinations with a strong emphasis on training loss and learning rate behavior.

Since it's impractical to run every configuration for the full 4000 epochs, I initially trained each setup for just 500 epochs. Configurations that showed a consistent decrease in training loss and maintained a high learning rate were preferred. A higher learning rate often indicates that the model hasn't yet plateaued, meaning there's still significant learning potential remaining.

below is the generated reply

![Image](https://github.com/user-attachments/assets/1d237bad-e932-47b5-bcaa-14de9086320a)
