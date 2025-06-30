# 🚀 AI-Violence-Detection-System

AI-powered real-time violence detection system for surveillance videos using deep learning and computer vision.


![License](https://img.shields.io/badge/License-MIT-blue)
![Python](https://img.shields.io/badge/Python-3.9+-yellow.svg)
![Frameworks](https://img.shields.io/badge/Frameworks-Flask%20%7C%20React%20%7C%20Laravel-green.svg)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange.svg)

---

## 📜 Abstract

This project presents an intelligent, deep learning-based system for detecting violence in video streams using spatiotemporal analysis. The system integrates a hybrid model combining **`MobileNetV2`** (for spatial feature extraction) with a **`Bidirectional LSTM`** (for temporal sequence modeling) to classify video segments as either violent or non-violent.

In addition to violence detection, the system includes modules for **🔥 Fire Detection (`YOLOv8`)** and **🧍 Real-time Person Tracking (`DeepSORT`)**, enhancing situational awareness. The system is supported by a scalable backend (`Laravel + Flask`) and a modern frontend (`React.js`), ensuring smooth integration, alert generation, and event reporting.

---

## 🎥 Live Demo

A live demonstration is the best way to showcase the system's capabilities.

_(This is the most crucial part of your README. Record a short GIF or video of your system in action and replace the placeholder below.)_

![System Demo GIF](https://github.com/andrew-atef/AI-Violence-Detection-System/blob/main/Demo/demo.gif)
_(Note: This is an example path. Please create a `Demo` folder in your repository, upload your GIF, and update the link.)_

---

## ✨ Key Features

- **💥 Real-time Violence Detection:** Classifies violent actions in live video streams using a `MobileNetV2 + BiLSTM` model.
- **🔥 Fire Detection:** An integrated module using `YOLOv8` to identify flames and smoke.
- **🧍 Person Tracking:** Employs the `DeepSORT` algorithm to track suspects after an incident is detected.
- **🚨 Instant Alerts & Reporting:** Automatically generates incident reports upon threat detection, visible on the admin dashboard.
- **⚙️ Scalable Architecture:** Built on a microservices-inspired architecture, decoupling the AI service from the main application logic.
- **👤 Comprehensive Dashboard:** An intuitive web interface for Admins and Employees to manage cameras, users, and monitor events.

---

## 🏛️ System Architecture

The system is designed with a multi-tiered architecture to ensure modularity, scalability, and maintainability.

1.  **Frontend (React.js):** A Single Page Application (SPA) that provides the user interface for monitoring live feeds, managing system resources, and viewing incident reports.
2.  **Backend (Laravel):** A central RESTful API that handles business logic, user authentication & authorization, and data persistence with the database.
3.  **AI Service (Flask):** A lightweight, dedicated microservice that exposes an API endpoint to receive video clips, run them through the deep learning models, and return predictions.

**Data Flow:**
`User (React)` ➡️ `Sends Video Clip` ➡️ `AI Service (Flask)` ➡️ `Processes & Returns Prediction` ➡️ `Triggers Report` ➡️ `Backend (Laravel)` ➡️ `Stores in DB` ➡️ `Displays on Dashboard`.

---

## 🛠️ Technology Stack

| Category                  | Technology / Framework                                  |
| ------------------------- | ------------------------------------------------------- |
| **Frontend**              | `React.js`, `Axios`                                     |
| **Backend**               | `Laravel (PHP)`, `MySQL`                                |
| **AI / ML Service**       | `Python`, `Flask`, `TensorFlow/Keras`, `OpenCV`         |
| **AI/ML Models**          | `MobileNetV2`, `BiLSTM`, `YOLOv8`, `DeepSORT`           |
| **Training & Deployment** | `Google Colab`, `Hugging Face Hub`, `Docker (Optional)` |



## ⚙️ Setup and Installation

To run the system locally, you need to set up the AI Service and the Frontend Application.

### 1. AI Service (Flask API)


## Clone the repository
git clone https://github.com/andrew-atef/AI-Violence-Detection-System.git
cd AI-Violence-Detection-System

## Create and activate a virtual environment (recommended)
python -m venv venv
# On Windows: venv\Scripts\activate
# On macOS/Linux: source venv/bin/activate

## Install dependencies
pip install -r requirements.txt

## NOTE: Ensure the trained model (.keras file) is available in the correct path.
# The script may download it from Hugging Face Hub if configured.

## Run the Flask server
python flask_app.py


## Clone the frontend repository
git clone https://github.com/AndrewSherif0/Violence-Detection-System.githup.io.git
cd Violence-Detection-System.githup.io

## Install dependencies
npm install

## Start the application
npm start


📁 Project Components
This project is distributed across several repositories and notebooks.
🔗 Main Repository (AI & Backend)
🔗 Frontend Repository
🔗 Model Training Colab Notebook
🔗 Flask API Colab Notebook
🔗 Full Project Documentation: (Upload your documentation PDF to GitHub and link it here)

🤝 Contributing
Contributions are welcome! If you'd like to improve the project, please follow these steps:
Fork the Project.
Create your Feature Branch (git checkout -b feature/AmazingFeature).
Commit your Changes (git commit -m 'Add some AmazingFeature').
Push to the Branch (git push origin feature/AmazingFeature).
Open a Pull Request.

## 👥 Project Team
### Abdallah Ashraf Abdallah - 20210541
### Andrew Atef Shukrallah - 20210191
### Andrew Sherif Shokry - 20210190
### Alaa Hesham Mamdouh - 20210173
### Zeina Samer Wagdy - 20210390
##Supervised by
### Dr. Hala
```
