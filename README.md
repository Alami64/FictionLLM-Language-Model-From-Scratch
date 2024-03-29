# FictionLLM-Language-Model-From-Scratch

FictionLLM is a language model based on the GPT (Generative Pre-trained Transformer) architecture, specifically inspired by GPT-2. It is designed to be trained on a large corpus of webfiction text data to generate webfiction like stories.

## Features

-Gradient accumulation for simulating larger batch sizes

-Learning rate scheduling with warmup and decay

-Model evaluation during training

-Checkpointing and resuming training from saved checkpoints

-Efficient training using PyTorch's torch.compile() feature (requires PyTorch 2.0)

## Usage

1. Prepare your dataset in the required format (train.bin and val.bin files) and place it in the data directory.
2. Configure the model and training settings in the configurator.py file or by passing command-line arguments to train.py.
3. Run the training script:
    ```bash
    python train.py
    ```
4. Monitor the training progress and evaluate the model's performance using the provided metrics.  
5. Once training is complete, the trained model checkpoint will be saved in the out directory.


## The model hyperparameters, such as the number of layers, number of attention heads, and embedding dimensions, can be customized in the configurator.py file or through command-line arguments.
