# Brain Tumor Detection Web Application

This project is a deep learning-based web application to detect brain tumors from MRI images using a Convolutional Neural Network (CNN) built in PyTorch. The application provides a user-friendly interface via Streamlit, allowing anyone to upload an MRI image and receive an instant prediction on whether a brain tumor is present.

## Features

- Upload MRI images (JPG or PNG)
- Real-time prediction of tumor presence
- Simple Streamlit interface for non-technical users
- PyTorch-based custom CNN model
- Pre-trained model weights included

## Demo

<!-- You can add screenshots of your Streamlit app here -->

## Installation

### Prerequisites

- Python 3.7 or higher
- pip

### Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/aiyenigbacharles/Brain-Tumor-Detection.git
   cd Brain-Tumor-Detection
   ```

2. **Install dependencies:**
   ```bash
   pip install streamlit torch torchvision pillow
   ```

3. **Model Weights:**
   - Ensure `brain_tumor_detector.pt` is in the project root. This is the pre-trained model weights file.

### Running the App

```bash
streamlit run deploy.py
```

Then open the provided local URL in your browser.

## Usage

1. Click "Browse files" to upload a brain MRI image (JPG or PNG).
2. Click "Predict" to get the result.
3. The app will display whether a tumor is detected or not.

## Project Structure

- `deploy.py` — Main Streamlit app for image upload and prediction
- `brain_tumor_detector.pt` — Pre-trained PyTorch model weights
- `brain_tumor_detector.h5` — (Optional/Legacy) Model weights in HDF5 format
- `tumor_detection.ipynb` — Jupyter Notebook for model training, validation, and testing

## Model Details

- A custom CNN with two convolutional layers, ReLU activations, max pooling, and two fully connected layers.
- Trained to classify MRI brain images as "tumor" or "no tumor".

## Technologies Used

- Python, PyTorch, Streamlit, PIL, torchvision

## Author

Charles Aiyenigba

## License

Charles License
