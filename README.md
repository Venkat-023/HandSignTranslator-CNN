Real-Time American Sign Language (ASL) Recognition Using CNN

HandSign-Translator is a real-time ASL alphabet recognition system that detects hand gestures from a webcam feed, classifies them using a custom-built Convolutional Neural Network (CNN), and dynamically constructs sentences based on confident predictions. The result is a smooth and intelligent system that bridges visual language and readable text.

📌 Project Highlights
🧠 Custom CNN architecture built from scratch

🎥 Real-time gesture recognition via webcam

✋ MediaPipe used for precise hand detection and dataset cleaning

⚪ Grayscale image processing for faster and more robust model inference

🧪 Trained on a self-curated dataset with over 94% testing accuracy

💬 Confidence-based sentence construction displayed live on-screen

🖼️ Dataset Preparation
Source: ASL alphabet dataset from Kaggle

Due to dataset size and noise, it was split and preprocessed in parts

MediaPipe was used to extract and crop only the hand region from images

Cleaned dataset was saved and converted to grayscale for better model performance

Final dataset was significantly smaller, cleaner, and optimized for CNN training

🧠 Model Architecture
Designed and trained 15+ custom CNN models

Used TensorFlow/Keras for model building and evaluation

Best-performing model achieved 94%+ accuracy on test data

Final model was exported and integrated into a real-time prediction pipeline

🎥 Real-Time Pipeline
Capture live video input using OpenCV

Detect hand region using MediaPipe

Preprocess the frame (resize & grayscale)

Predict gesture using the trained CNN

Validate prediction confidence

Build sentence from validated predictions

Display the result live on the webcam feed

⚙️ Technologies Used
Python 3.x

TensorFlow / Keras

OpenCV

MediaPipe

NumPy, Matplotlib

📦 Use Cases
ASL learning tools and educational platforms

Assistive communication for individuals with speech or hearing impairments

Research in gesture recognition and HCI (Human-Computer Interaction)

Gesture-based user interfaces and control systems

🎯 Future Enhancements
Extend support to ASL words and phrases

Add multi-hand support for more complex gestures

Improve UI/UX with overlay controls and customization

Export as a lightweight desktop app using PyInstaller or Electron

