# Egyptian ID Card Address Extraction with OCR

## Project Overview

This project uses Optical Character Recognition (OCR) to accurately extract address information from Egyptian national ID cards. The core of the solution is a powerful **Convolutional Recurrent Neural Network (CRNN)** model combined with the **Connectionist Temporal Classification (CTC) loss function** to handle variable-length text sequences.

## Key Features

* **High Accuracy**: Achieves a high degree of accuracy in recognizing and extracting Arabic text addresses.
* **Robust Architecture**: Utilizes a combination of CNN for feature extraction and RNN (specifically LSTM) for sequence modeling, making it effective for a wide range of text layouts.
* **CTC Loss**: Employs CTC loss to handle text with different lengths without the need for a pre-segmented dataset, which simplifies the training process.
* **Gradio Integration**: Includes a simple user interface built with Gradio, allowing users to upload an image of an ID card and get the extracted address instantly.

## How It Works

The project follows a standard OCR pipeline:

1.  **Data Preprocessing**: Images are loaded, converted to grayscale, and normalized to ensure consistency.
2.  **Text Cleaning**: The text data is cleaned to prepare it for training.
3.  **Model Training**: The CRNN model is trained on a dataset of Egyptian addresses. The CTC loss function is crucial here for aligning the predicted sequences with the ground truth labels.
4.  **Inference and Decoding**: The trained model processes new images, and a decoding mechanism is used to convert the model's output into a readable text string.

## Getting Started

### Prerequisites

* Python 3.x
* A package manager like `pip`


## Potential Impact

This project has significant potential to **transform administrative tasks** in government offices and private institutions in Egypt. By automating the extraction of addresses from ID cards, this OCR solution can:

  * **Reduce processing time**: Instead of typing addresses, clerks can simply scan the ID, and the address is automatically populated into the system.
  * **Minimize data entry errors**: Automated processes are far more accurate than manual ones, leading to higher data quality.
  * **Improve efficiency**: Frees up staff to focus on more complex tasks, enhancing overall productivity and service quality.

This technology can also be integrated into mobile applications for quick verification or data capture, providing a more modern and streamlined experience for citizens and employees alike.
