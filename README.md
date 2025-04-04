# 🎤 Sonic Lip Sync - Gradio App (Google Colab Setup)

This project brings the [Sonic](https://github.com/jixiaozhong/Sonic) lip-sync model into a user-friendly Gradio interface, allowing you to generate realistic lip-synced videos directly in **Google Colab** using Hugging Face models. No local installation required.

---

## 🚀 Demo
Launches a `.gradio.live` URL from Colab to interact with the app in your browser.

---

## 🧰 Features
- 🔊 Converts images and audio into lip-synced video
- 🤖 Powered by: `Sonic`, `Stable Video Diffusion`, `Whisper-tiny`
- 🌐 Hosted in Google Colab with full CUDA and PyTorch support
- 🧠 Uses Hugging Face CLI to fetch model checkpoints

---

## ⚙️ Setup Instructions (Google Colab)

### 🗂️ 1. Clone the Project in Colab
```bash
mkdir ai-tools
cd ai-tools
mkdir sonic-lip-sync
cd sonic-lip-sync
git clone https://github.com/jixiaozhong/Sonic.git
cd Sonic
```

### 🗂️ 2. Install Dependencies
```bash
pip install -r requirements.txt
pip install opencv-python
```

### 🗂️ 3. Install PyTorch with CUDA 12.6
```bash
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu126
```

### 🗂️ 2. Install Dependencies
```bash
pip install -r requirements.txt
pip install opencv-python
```

