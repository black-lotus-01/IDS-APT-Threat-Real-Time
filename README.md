# 🔒 Real-time Intrusion Detection Web App

<b>Developed by: Barq Ahmed</b><br> <b>Project: Intelligent IDS using Deep Learning (CNN)</b><br>

---

## 🧠 About

This project implements a **Real-Time Intrusion Detection System (IDS)** powered by **Deep Learning** and a **Flask Web Interface**.

It uses a **Convolutional Neural Network (CNN)** model trained on the **KDD dataset** to detect and classify malicious network activities in real time.

### 🎯 Key Features

* Real-time network intrusion detection
* Deep Learning (CNN) model for classification
* Flask-based responsive web dashboard
* User-friendly interface for live prediction
* Supports custom datasets (extendable to CICIDS2018, NSL-KDD, etc.)

---

## ⚙️ System Overview

The IDS processes live or user-input network features, classifies them using the trained CNN model, and provides the output through an interactive web app.

**System Architecture Diagram:**

```
Network Data  →  Preprocessing  →  CNN Model  →  Flask Web App  →  Real-time Results
```

---

## 🖥️ Requirements

1. **Windows OS**

2. **Python 3.9**
   *Download links:*

   * [Python 3.9 (64-bit)](https://www.python.org/ftp/python/3.9.13/python-3.9.13-amd64.exe)

   * [Python 3.9 (32-bit)](https://www.python.org/ftp/python/3.9.13/python-3.9.13.exe)

   > **Note:** During installation, select **“Add Python 3.9 to PATH”**.

3. **Dependencies:**
   Automatically installed from `requirements.txt`:

   ```bash
   flask
   flask-wtf
   tensorflow
   pandas
   numpy
   scikit-learn
   ```
4. **Npcap 1.71:** https://npcap.com/dist/npcap-1.71.exe
---

## 🧩 Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/black-lotus-01/Intrusion-Detection-System.git
cd Intrusion-Detection-System-main
```

### 2️⃣ Create Virtual Environment

```bash
python -m venv venv
```

### 3️⃣ Activate the Environment

**Windows:**

```bash
venv\Scripts\activate
```

**Linux/Mac:**

```bash
source venv/bin/activate
```

### 4️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 5️⃣ Run the Application

```bash
python run.py
```

Access the web app at 👉 **[http://localhost:5000](http://localhost:5000)**

---

## 🧠 Model Description

The **CNN model (`System/codeCNN.py`)** is trained using the **KDDTrain.csv** dataset.
It classifies network connections into several categories such as:

* **Normal**
* **Denial of Service (DoS)**
* **Probe**
* **R2L (Remote to Local)**
* **U2R (User to Root)**

### 🧩 Learned Features

The model learns and processes essential network traffic features such as:

* Protocol type
* Service
* Flag
* Source and destination bytes
* Duration and count metrics

---

### 🏠 Main Interface

Displays a form to input network parameters for detection.

![Interface Example](https://github.com/black-lotus-01/IDS-APT-Threat-Real-Time/raw/main/images/image1.png)

### 📊 Prediction Results Page

Shows classification output (Normal / Attack type).

![Interface Example](https://github.com/black-lotus-01/IDS-APT-Threat-Real-Time/raw/main/images/image2.png)
---

## 🔮 Future Improvements

* Integrate with **live packet capture (Wireshark / Npcap)**
* Add **REST API endpoints** for remote detection
* Enhance **visual analytics dashboard**
* Extend dataset with **CICIDS 2018** and **custom network traffic**

---

## 👨‍💻 Author

**Barq Ahmed**
Cybersecurity & AI Researcher
📧 [official.cyber010@gmail.com](mailto:official.cyber010@gmail.com)
🌐 [GitHub: black-lotus-01](https://github.com/black-lotus-01)

---

## 📜 License

This project is released under the **MIT License**.
You are free to use, modify, and share it with proper attribution.

