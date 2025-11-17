🧠 Object Classification Using OpenCV & TensorFlow

A complete end-to-end pipeline for building your own custom object classifier using your webcam.
This project allows you to:

✔ Capture your own dataset
✔ Train a CNN model
✔ Run real-time object recognition

Everything is done using OpenCV + TensorFlow.

📌 Features

Webcam-based dataset collection with a clean ROI box

Automatically stores images category-wise

Data augmentation during training

Lightweight CNN model (easy to train on CPU)

Real-time object detection using the trained model

Easy to customize with your own classes

📁 Project Structure
│── dataset/
│   ├── mobile/
│   ├── bottle/
│   ├── book/
│   ├── headphone/
│   └── mouse/
│
│── data_collection.py
│── train_model.py
│── realtime_prediction.py
│── object_model.h5
│── README.md

🎥 1. Dataset Collection

Use the webcam to capture images for each class.

Keys

c → Capture image

n → Next class

q → Quit

The script automatically creates folders and saves 128×128 cropped images.

🧠 2. Model Training

The training script uses:

Convolutional Neural Networks (CNN)

Image augmentation

Train-validation split

Softmax layer for multi-classification

Output model is saved as:

object_model.h5

🖥️ 3. Real-Time Prediction

After training, run the real-time script to classify objects placed inside the ROI box.

🔧 Requirements

Install the required packages:

pip install opencv-python tensorflow numpy

🚀 How to Run
1️⃣ Collect Dataset
python data_collection.py

2️⃣ Train the Model
python train_model.py

3️⃣ Predict in Real-Time
python realtime_prediction.py

🛠️ Customization

To add more classes:

Add them in the classes = [] list

Collect images

Retrain the model

📌 Future Improvements

Switch to MobileNetV2 for higher accuracy

Add sound/vibration feedback on capture

Add GUI for data collection

Deploy as a desktop app

🤝 Contributions

Feel free to fork the repo and create pull requests!

📜 License

MIT License (open for everyone)
