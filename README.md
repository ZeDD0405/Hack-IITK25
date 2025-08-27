
# 🔐 AI-Driven Insider Threat Detection System

**🏆 Winner – 1st Prize at HackIITK 2025**
Beating 7000+ participants from BTech, MTech, and international universities

---

## 📌 Project Overview

**AI-Driven Insider Activity Detection System** is an end-to-end **AI + Cybersecurity** solution designed to **detect, monitor, and report insider threats in real-time**.
It combines **packet-level data analysis, machine learning models, and an interactive SOC dashboard** for security analysts.
<img width="1903" height="902" alt="dashboard" src="https://github.com/user-attachments/assets/8d503218-5b51-4ead-b8ba-ab8e394fc768" />



---

## 🎯 Core Objectives

1. **Robust AI-based detection** of insider threats from activity logs & network packets.
2. **Real-time, intuitive dashboard** for cybersecurity teams.
3. **Automated report generation & alerts** for faster incident response.

---

## ⚡ Key Features

### 🔎 Real-Time Detection

* **Packet Sniffing** with `Scapy` for live capture.
* **Streaming & Buffering** using `Apache Kafka` for scalable ingestion.
* **XGBoost Model** for fast binary classification of anomalies (batch of 50 packets).

### 🤖 Deep Anomaly Detection

* **Autoencoder Neural Network** trained on 13GB+ insider activity dataset.
* **Dask** for distributed feature engineering on GPU (Google Colab T4).

### 📧 Email Threat Analysis

* **VirusTotal API** integration for detecting phishing/malware in email payloads.

---

## 🖥️ Interactive Dashboard (Next.js)

* Real-time alerts with severity indicators.
* Downloadable `.pcap` logs for forensic analysis.
* Incident tracking & analyst assignment.
* Timeline visualization of suspicious behavior.
* Modern, responsive SOC dashboard UI.

---

## 🛠️ Tech Stack

| Component         | Technology           |
| ----------------- | -------------------- |
| Packet Capture    | Scapy                |
| Stream Processing | Apache Kafka         |
| AI Models         | XGBoost, Autoencoder |
| Dashboard         | Next.js              |
| Backend/API       | FastAPI              |
| Data Processing   | Dask, Pandas         |
| Email Scanning    | VirusTotal API       |
| Model Training    | Google Colab (GPU)   |

---

## 🚀 Challenges & Solutions

| Challenge                       | Solution                                  |
| ------------------------------- | ----------------------------------------- |
| High-volume data processing     | Dask + Colab T4 GPU for parallelization   |
| Real-time packet flood handling | Batch-based anomaly analysis (50 packets) |
| Analyst usability               | Built clean, modular Next.js dashboard    |

---

## ⚡ Setup Instructions

```bash
# Clone the repo
git clone https://github.com/yourusername/insider-threat-detection.git
cd insider-threat-detection

# Start backend (FastAPI)
cd backend
pip install -r requirements.txt
uvicorn main:app --reload

# Start frontend (Next.js)
cd ../dashboard
npm install
npm run dev
```

---

