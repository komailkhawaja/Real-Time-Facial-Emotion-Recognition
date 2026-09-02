# Real-Time Facial Emotion Recognition

A deep learning project that detects human facial emotions in real time using a webcam. The system is trained on the FER-2013 facial expression dataset and uses a Convolutional Neural Network (CNN) to classify seven emotions.

## Features

- Facial emotion classification using a CNN
- FER-2013 dataset
- Seven emotion classes:
  - Angry
  - Disgust
  - Fear
  - Happy
  - Neutral
  - Sad
  - Surprise
- Training and validation performance visualization
- Classification report and confusion matrix
- Real-time webcam emotion detection
- Confidence score for detected emotions
- Most common detected emotion and average confidence summary

## Technologies

- Python 3.12
- TensorFlow / Keras
- OpenCV
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Pillow
- Jupyter Notebook

## Project Structure

```text
Real-Time-Facial-Emotion-Recognition/
│
├── Emotion_Recognition.ipynb
├── README.md
├── requirements.txt

```

## Dataset

This project uses the **FER-2013** facial expression dataset.

The dataset contains facial images organized into seven emotion categories. The images are commonly provided at 48×48 resolution.

The dataset is intentionally not included in this repository because of its size. Download the dataset separately and place it in the expected folder structure:

```text
archive/
├── train/
│   ├── angry/
│   ├── disgust/
│   ├── fear/
│   ├── happy/
│   ├── neutral/
│   ├── sad/
│   └── surprise/
│
└── test/
    ├── angry/
    ├── disgust/
    ├── fear/
    ├── happy/
    ├── neutral/
    ├── sad/
    └── surprise/
```

Update the dataset path in the notebook if your dataset is stored somewhere else.

## Model

The project uses a custom CNN containing convolutional layers, batch normalization, max pooling, dropout, and fully connected layers.

The final layer uses a softmax activation to produce probabilities for the seven emotion classes.

## Running the Project

### 1. Clone the repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd Real-Time-Facial-Emotion-Recognition
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Open the notebook

```bash
jupyter notebook
```

Open:

```text
Emotion_Recognition.ipynb
```

### 4. Dataset

Download FER-2013 and arrange the folders according to the structure shown above.

Update:

```python
DATASET_PATH = r"C:\Users\HP\Desktop\archive"
```

to your own dataset location.

### 5. Train the model

Run the notebook cells in order. The trained model is saved as:

```text
emotion_model.keras
```

### 6. Real-time detection

Run the webcam section of the notebook.

The system uses the laptop webcam to detect faces and classify their expressions.

## Results

Add your final training graphs, confusion matrix, and webcam screenshot to the `screenshots/` folder.

Recommended files:

- `training_results.png`
- `confusion_matrix.png`
- `webcam_detection.png`

## Future Improvements

- Improve accuracy with transfer learning
- Add temporal smoothing to reduce frame-to-frame prediction changes
- Support multiple faces simultaneously
- Display all seven emotion probabilities
- Use a more advanced face detector
- Deploy the model as a web application

## Author

**Muhammad Komail Khawaja**

BS Artificial Intelligence

---

If you use or modify this project, please provide appropriate attribution to the original FER-2013 dataset and its creators.
