# Image Captioning with Visual Attention

## Overview
This project develops an image captioning model combining Convolutional Neural Networks (CNNs) and Long Short-Term Memory (LSTMs) with an attention mechanism. The model generates descriptive captions for images by dynamically focusing on different image parts during the caption formation. This model was coded from scratch, showcasing a custom implementation of both the neural networks and attention mechanisms.

## Data Preparation
Images and captions are preprocessed through resizing, normalization, and feature extraction using pretrained CNN models like EfficientNet or ResNet. Text data involves tokenization, vocabulary building, and sequence padding.

## Model Architecture
- **Feature Extraction**: Uses a pretrained CNN to convert images into feature vectors.
- **Caption Generation**: An LSTM network processes these features to generate captions word by word.
- **Attention Mechanism**: Dynamically focuses on different image regions for each word, enhancing contextual understanding.

## Training Process
Training uses Categorical Cross-Entropy Loss and the Adam optimizer. The process includes passing image features to generate word sequences and updating weights to match the generated captions with ground truth. This entire training process was built from the ground up to optimize for the best possible results.

## Evaluation
Performance is evaluated using BLEU scores, with results demonstrating the attention mechanism's impact on improving caption accuracy and relevance.

## Deployment & Future Scope
The model can be deployed using TensorFlow Serving or a Flask API. Future improvements may include training on larger datasets, adopting Transformer-based models, and extending to video captioning.

## Fun Experiment
For a bit of fun, I tried captioning my own photo with the model! It was exciting to see how the model interpreted a personal image.

## Acknowledgments
- Credits to Inspirational sources and references
