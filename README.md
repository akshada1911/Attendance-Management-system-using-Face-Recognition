# 🏫 Face Recognition-Based Attendance System  

This project automates **attendance tracking** using **face recognition technology**. It captures **real-time facial images**, processes them with **OpenCV and a machine learning model (KNN)**, and maintains attendance records with **Flask-based web integration**.  

---

## 📌 Table of Contents  
- [Introduction](#introduction)  
- [Problem Statement](#problem-statement)  
- [Importance of This Project](#importance-of-this-project)  
- [Methodology](#methodology)  
- [Results and Performance](#results-and-performance)  
- [Conclusion](#conclusion)  

---

## 📖 Introduction  
Traditional attendance systems **require manual input**, making them **time-consuming and prone to errors**. This project automates attendance using **face recognition** by capturing **live webcam footage**, detecting faces, and **marking attendance automatically**.  

---

## ❌ Problem Statement  
Manual attendance systems are:  
- **Time-consuming & inefficient**  
- **Prone to proxy attendance (buddy punching)**  
- **Difficult to manage for large groups**  

This project **automates** attendance using **AI-based face recognition** for **accurate, tamper-proof records**.  

---

## 🌍 Importance of This Project  
✅ **Automated Attendance**: Eliminates **manual efforts**  
✅ **Prevents Proxy Attendance**: Ensures **identity verification**  
✅ **Efficient Record-Keeping**: Stores attendance in **CSV format for easy access**  

---

## ⚙️ Methodology  

### 📌 Data Collection & Preprocessing  
- **Face Detection**: Uses `haarcascade_frontalface_default.xml` for face detection  
- **Face Image Processing**: Converts images to **grayscale** and **resizes** them to `(50×50)`  
- **Dataset Storage**: Captured faces are stored in `static/faces/`  

### 📌 Model Training  
- **Algorithm Used**: **K-Nearest Neighbors (KNN)**  
- **Feature Extraction**: Converts **face images into feature vectors**  
- **Model Storage**: Trained model saved as `face_recognition_model.pkl`  

### 📌 Attendance Marking  
- **Face Recognition**: Matches detected faces with stored **face embeddings**  
- **Timestamping**: Marks attendance with **Name, Roll No, and Time**  
- **Data Storage**: Attendance saved as `Attendance/Attendance-DD-MM-YY.csv`  

### 📌 Flask Web Integration  
- **Home Page**: Displays **attendance records**  
- **Take Attendance**: Captures real-time webcam feed for recognition  
- **Add User**: Registers new users by capturing **50 face images**  

### 📌 Training Process  

| Parameter | Value |  
|-----------|--------|  
| **Model** | KNN (K-Nearest Neighbors) |  
| **Face Image Size** | 50×50 |  
| **Dataset Path** | `static/faces/` |  
| **Feature Extraction** | Flattened pixel values |  
| **Classifier** | `KNeighborsClassifier(n_neighbors=5)` |  

---

## 📊 Results and Performance  

✅ **Accuracy**  
✔ Face recognition **accuracy** improved with **more training samples**  

✅ **Efficiency**  
✔ Attendance **marked in real-time**, reducing **processing delay**  

✅ **Scalability**  
✔ Can be expanded for **large organizations and classrooms**  

---

## 🏁 Conclusion  
- **Face recognition technology automates attendance**, making it **efficient & reliable**  
- **Real-time detection & recognition** ensure **fast processing**  
- **Flask integration provides a user-friendly interface** for monitoring attendance  

---
