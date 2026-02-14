# 🦺 PPE Detection System using YOLOv8

This project focuses on building a **Personal Protective Equipment (PPE) detection system** using a fine-tuned **YOLOv8n** model. The goal is to automatically detect whether workers are wearing the required safety equipment in industrial environments.

---

### 📌 Key Features
* **Detection of 15 safety-wear classes:** Includes helmets, vests, gloves, masks, and more.
* **Combined Dataset:** Model trained using images from several open-source PPE datasets (primarily Roboflow).
* **Real-time Support:** Detection supported through webcam or video streams.
* **Edge Ready:** Lightweight YOLOv8n model suitable for devices like Raspberry Pi.

---

### 🚀 Model Training
* **Offline Training:** Performed on static images, not CCTV footage, to ensure high-quality annotations.
* **Generalization:** Merges data from different sources to create a versatile training set.
* **Optimization:** Performance can be significantly improved by adding real images from your specific company (same cameras, environment, and lighting).

---

### 🎥 Real-Time Inference
The trained YOLOv8n model works with both single images and live video. A real-time demo was successfully tested using a standard laptop webcam.

---

### 🧩 Deployment
The model is hardware-flexible and can run on:
* **Standard Computer:** Uses CPU or GPU (GPU boosts speed significantly).
* **Raspberry Pi:** Performance improves greatly when using a **Google Coral TPU**.
* **No GPU Required:** While a GPU is recommended for high FPS, it is not strictly required for inference.

---

### 🛠️ Quick Start
1. **Install Dependencies:**
   ```bash
   pip install ultralytics opencv-python
