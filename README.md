# Traffic Sign Recognition Web Application

This project is a web-based application for recognizing traffic signs using a trained deep learning model. It allows users to upload images of traffic signs and receive predictions about the sign's class.

## Features
- Upload images of traffic signs for recognition
- Uses a pre-trained Keras model (`model.h5`)
- Web interface built with Flask
- Dataset organized by class in the `Dataset/` directory

## Project Structure
```
app.py                # Main Flask web application
main.py               # Model training or utility script
model.h5              # Trained Keras model
labels.csv            # CSV file mapping class indices to sign names
Dataset/              # Traffic sign images organized by class
static/               # Static files (CSS, JS)
templates/            # HTML templates
uploads/              # Uploaded images
```

## Getting Started

### Prerequisites
- Python 3.7+
- pip
- Required Python packages (see below)

### Installation
1. Clone the repository:
   ```sh
   git clone <repo-url>
   cd traffic-sign-recognition-web
   ```
2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
   If `requirements.txt` is missing, install manually:
   ```sh
   pip install flask keras tensorflow pillow numpy pandas
   ```

### Running the App
1. Start the Flask server:
   ```sh
   python app.py
   ```
2. Open your browser and go to `http://127.0.0.1:5000/`

## Usage
- Upload a traffic sign image via the web interface.
- The app will display the predicted class and sign name.

## Dataset
- The `Dataset/` folder contains subfolders for each class (0, 1, 2, ...), each with images of that class.
- `labels.csv` maps class indices to human-readable sign names.

## Model
- The model is stored in `model.h5` and is loaded by the Flask app for predictions.
- To retrain or update the model, use `main.py` (if implemented for training).

## License
This project is for educational purposes.
