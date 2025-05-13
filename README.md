

# 🎉 **YourAI: Revolutionizing Healthcare with Intelligence** 🤖💉

![YourAI Logo](https://image.shutterstock.com/image-vector/ai-medicine-outline-icon-simple-600nw-2523986339.jpg)

---

## 🎯 **Vision**

YourAI is a next-generation healthcare assistant that transforms how we interact with our health data. Powered by cutting-edge AI and natural language processing, it delivers an intuitive, accessible, and personalized healthcare experience for everyone.

---

## ✨ **Core Features**

### 🤝 **Intelligent Interaction**

* 💬 **Natural Conversations**: Human-like dialogues for health guidance.
* 🎙️ **Voice Commands**: Manage health tasks hands-free.
* 📧 **Email Management**: Stay organized with health-related emails.
* 📅 **Calendar Sync**: Book appointments with simple voice commands.
* 🧠 **Smart Responses**: Clear and insightful health advice.

### 🔗 **Seamless Integration**

* 🌐 **Google Workspace**: Effortless integration with Gmail and Google Calendar.
* 🌙 **Dark Mode**: Comfortable, eye-friendly interface anytime.
* 📚 **History Tracking**: Access your health conversations anytime.
* 📱 **Cross-Platform**: Works beautifully on all devices.

---

## 🛠️ **Technology Stack**

| Layer      | Tech Stack                     |
| ---------- | ------------------------------ |
| Frontend   | React.js, Next.js, TypeScript  |
| Voice      | Web Speech API, Piper, WaveNet |
| AI Engine  | Llama 3.1 Model                |
| Backend    | Node.js, Express, PostgreSQL   |
| Deployment | Docker, AWS, GitHub Actions    |

---

## 🚀 **Quick Start Guide**

### 📋 **Prerequisites**

* Node.js (v14+)
* npm (v6+)
* Google Cloud Platform account
* OAuth 2.0 credentials

### 📦 **Installation**

```bash
git clone https://github.com/your-username/yourai-health.git
cd yourai-health
npm install
```

📄 **Create `.env.local`**

```env
NEXT_PUBLIC_API_URL=your_api_url
NEXT_PUBLIC_GOOGLE_CLIENT_ID=your_client_id
GOOGLE_CLIENT_SECRET=your_client_secret
PIPER_PATH=/path/to/piper/build/piper
PIPER_MODEL_PATH=/path/to/piper/models/en_US-libritts-high.onnx
```

---

## 🎙️ **Voice System Setup (Piper)**

```bash
git clone https://github.com/rhasspy/piper.git
cd piper
mkdir build && cd build
cmake ..
make
```

Download Voice Model:

```bash
curl -L -o models/en_US-libritts-high.onnx https://huggingface.co/rhasspy/piper-voices/resolve/v1.0.0/en/en_US/libritts/high/en_US-libritts-high.onnx
curl -L -o models/en_US-libritts-high.onnx.json https://huggingface.co/rhasspy/piper-voices/resolve/v1.0.0/en/en_US/libritts/high/en_US-libritts-high.onnx.json
```

Install Dependencies:

```bash
brew install espeak-ng
```

---

## 🔐 **Google API Integration**

1. Navigate to [Google Cloud Console](https://console.cloud.google.com/).
2. Create/Select a Project → Enable APIs → Generate Credentials.
3. Required Scopes:

   * `https://www.googleapis.com/auth/gmail.readonly`
   * `https://www.googleapis.com/auth/calendar.events`

---

## 💬 **Using YourAI**

* **Wake Word**: "Hey YourAI" or "Hello"
* 📧 **Emails**: "Check my health emails"
* 📅 **Appointments**: "Schedule a checkup for tomorrow"

---

## 🧠 **System Architecture**

```
┌────────────────┐      ┌───────────────────┐
│  Text Thread   │◄────►│   Audio Thread    │
└────────────────┘      └───────────────────┘
    │  ┌──────────────┐      ┌──────────────┐
    └─►│ AI Responses │      │ Voice Synthesis │
       └──────────────┘      └──────────────┘
```

---

## 🎓 **Custom Voice Training**

1. 📥 **Data Collection**: `audio_download_create_wav_files.py`
2. 🧹 **Data Cleaning**: `process_wav_files_to_remove_wav_errors.py`
3. 📜 **Transcription**: Use Whisper with `transcript.py`
4. 🎛️ **Model Training**: [Training Notebook](https://colab.research.google.com/github/rmcpantoja/piper/blob/master/notebooks/piper_multilingual_training_notebook.ipynb)

---

## 💻 **Development**

```bash
npm run dev
```

---

## 🤝 **Contributing**

We welcome your contributions to transform healthcare together!

1. 🍴 Fork the repository
2. 📂 Create a feature branch
3. ✅ Commit your changes
4. 📤 Push and open a Pull Request

---

## 🌟 **About YourAI**

YourAI was developed during the Princeton University Hackathon by a team passionate about solving real healthcare challenges. With a vision of **accessible, AI-powered healthcare for everyone**, YourAI centralizes health records, enhances medication management, streamlines insurance processes, and safeguards personal data privacy.

---

<div align="center">
  <h3>🚀 Join the Healthcare Revolution!</h3>
  <p>Empowering healthier lives, one interaction at a time.</p>
</div>

---

