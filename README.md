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

## ⚙️ Setup Instructions

### 🗂️ 1. Clone the Project in Colab
```bash
mkdir ai-tools
cd ai-tools
mkdir sonic-lip-sync
cd sonic-lip-sync
git clone https://github.com/jixiaozhong/Sonic.git
cd Sonic
```

### 🧪 2. Create a Virtual Environment (Not required if using Colab or any hosted Environement)
```bash
python -m venv venv
call venv\scripts\activate
```

### ⚙️ 3. Install CUDA Toolkit 12.6 (recommended version 12.6)
```bash
conda install nvidia/label/cuda-12.6.2::cuda-toolkit
```

### 📄 4. View and update the requirements.txt
```bash
cat requirements.txt
```
- remove the torch commands (total 3)
  

### 🔥 5. Install PyTorch with CUDA 12.6
```bash
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu126
```

### 📦 6. Install the requirements.txt
```bash
pip install -r requirments.txt
```

### 🤗 7. Install and download Hugging Face CLI Models
```bash
python -m pip install "huggingface_hub[cli]"

huggingface-cli download LeonJoe13/Sonic --local-dir checkpoints
huggingface-cli download stabilityai/stable-video-diffusion-img2vid-xt --local-dir checkpoints/stable-video-diffusion-img2vid-xt
huggingface-cli download openai/whisper-tiny --local-dir checkpoints/whisper-tiny
```

### 🧩 8. Install remaining dependencies
```bash
pip install opencv-python
pip install accelerate
```

### 📝 9. Open and Update the gradio_app.py
- Go to the end of the file.
- Replace the server from 0.0.0.0 to 127.0.0.1

### ▶️ 10. Run the Application
```bash
python gradio_app.py
```



