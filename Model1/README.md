We used the following dataset for our image processing and caption generation project:

Dataset Link
https://www.kaggle.com/datasets/raddar/chest-xrays-indiana-university
What We Do with the Data

This project focuses on image processing and automatic caption generation using machine learning techniques. The overall workflow consists of several steps, each detailed below.
1. Preprocessing the Images

To prepare the dataset for analysis, we perform various preprocessing tasks, such as:

    Resizing images to a consistent dimension for input to the model.
    Normalization to scale pixel values to a suitable range.
    Noise reduction to remove unwanted artifacts from the images.


2. Feature Extraction

We use deep learning techniques, particularly Convolutional Neural Networks (CNNs), to extract meaningful features from the images. This involves passing the images through layers of convolution, pooling, and activation functions to capture patterns such as edges, textures, and shapes.


3. Caption Generation

Once the features are extracted, we use a combination of a CNN and a Recurrent Neural Network (RNN) to generate captions. The CNN extracts visual features, while the RNN (typically using LSTM or GRU) translates these features into a sequence of words, producing a relevant caption for each image.


4. Evaluation

We evaluate the generated captions using metrics such as:

    BLEU Score: Measures how closely the generated caption matches the reference caption.
    ROUGE Score: Evaluates recall by comparing the overlap between generated and reference words.
    CIDEr Score: Custom metric designed for captioning tasks.


Pipeline Summary

Our end-to-end pipeline takes raw images as input, and processes them through multiple stages of preprocessing, feature extraction, and caption generation, resulting in a descriptive caption for each image. Below is a visual summary of the process:

