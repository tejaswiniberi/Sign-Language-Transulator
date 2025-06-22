# 🤟 Sign Language Translator

The **Sign Language Translator** is a Python-based deep learning project that interprets American Sign Language (ASL) hand gestures using a webcam and translates them into English alphabets. It uses **OpenCV**, **MediaPipe**, and **TensorFlow/Keras** to detect and recognize hand signs in real-time, helping bridge the communication gap for the deaf and hard-of-hearing community.

---

## 📌 Features

- 🎥 Real-time ASL gesture recognition using webcam
- 🧠 Convolutional Neural Network (CNN) for classification
- ✋ Hand detection powered by MediaPipe
- 💾 Easy-to-use dataset collection tool
- 🖥 Visual prediction display using OpenCV

---

## 🛠 Tech Stack

- **Python 3.x**
- **TensorFlow / Keras**
- **OpenCV**
- **MediaPipe**
- **NumPy**
- **Matplotlib**

---

## 📁 Project Structure
sign-language-translator/
│
├── dataset/ # Folder containing gesture images A-Z
│ ├── A/, B/, C/, ... # Subfolders for each alphabet
│
├── model/ # Trained model
│ └── asl_model.h5
│
├── collect_dataset.py # Script to collect hand gesture images
├── train_model.py # Script to train the CNN model
├── predict.py # Script for real-time predictions
├── requirements.txt # List of Python dependencies
├── README.md # Project documentation

## 🚀 How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/sign-language-translator.git
cd sign-language-translator

2. Create a Virtual Environment (Optional)
python -m venv venv
# Activate the virtual environment
venv\Scripts\activate      # On Windows
source venv/bin/activate   # On Linux/macOS

3. Install Dependencies
pip install -r requirements.txt
## If requirements.txt is not available, manually install:
pip install opencv-python mediapipe tensorflow numpy matplotlib

📸 Collect the Dataset
Capture images for each ASL alphabet (A-Z) using your webcam:
python collect_dataset.py

🧠 Train the Model
Once the dataset is collected, run:
-> python train_model.py
This will train a CNN and save the model as model/asl_model.h5

🤖 Run Real-Time Prediction
To run the live sign language translator using webcam:
python predict.py

🖼 Sample Output
✋ Detected → B
🤙 Detected → Y
👌 Detected → F

💡 Future Enhancements
🔠 Full sentence recognition
📚 Add support for dynamic gestures and words
🌐 Multi-language translation support
🧩 GUI-based interface using Tkinter or PyQt
