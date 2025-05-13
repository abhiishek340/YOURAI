# YourAI: Revolutionizing Healthcare with Intelligence 🤖💉

![YourAI Banner](https://via.placeholder.com/1200x400?text=YourAI+Healthcare+Assistant)

## 🎯 Vision

YourAI is a next-generation healthcare assistant that transforms how we interact with our health data. By leveraging cutting-edge artificial intelligence and natural language processing, we're creating a more intuitive, accessible, and personalized healthcare experience for everyone.

## ✨ Core Capabilities

### 🤝 Intelligent Interaction
- **Natural Dialogue**: Experience human-like conversations for health guidance
- **Voice Commands**: Control your health assistant hands-free
- **Smart Responses**: Get clear, natural-sounding health advice
- **Email Integration**: Manage health-related communications effortlessly
- **Calendar Sync**: Schedule appointments with simple voice commands

### 🔄 Seamless Integration
- **Google Workspace**: Connect with Calendar and Gmail
- **Dark Mode**: Eye-friendly interface for all hours
- **History Tracking**: Access your health conversations anytime
- **Cross-Platform**: Use on any device with responsive design

## 🛠️ Technical Foundation

### Frontend Architecture
- **Framework**: React.js with TypeScript
- **Performance**: Next.js optimization
- **Voice Tech**: Web Speech API integration
- **AI Engine**: Advanced Llama 3.1 Model
- **Voice Generation**: Piper and WaveNet synthesis

## 🚀 Quick Start Guide

### Prerequisites
- Node.js (v14+)
- npm (v6+)
- Google Cloud Platform account
- OAuth 2.0 credentials

### Installation Steps

1. **Clone and Setup**
   ```bash
   git clone https://github.com/your-username/yourai-health.git
   cd yourai-health
   ```

2. **Dependencies**
   ```bash
   npm install
   ```

3. **Environment Setup**
   Create `.env.local`:
   ```
   NEXT_PUBLIC_API_URL=your_api_url
   ```

## 🎙️ Voice System Setup

### Piper Integration
1. **Build Process**
   ```bash
   git clone https://github.com/rhasspy/piper.git
   cd piper
   mkdir build && cd build
   cmake ..
   make
   ```

2. **Model Installation**
   ```bash
   curl -L -o models/en_US-libritts-high.onnx https://huggingface.co/rhasspy/piper-voices/resolve/v1.0.0/en/en_US/libritts/high/en_US-libritts-high.onnx
   curl -L -o models/en_US-libritts-high.onnx.json https://huggingface.co/rhasspy/piper-voices/resolve/v1.0.0/en/en_US/libritts/high/en_US-libritts-high.onnx.json
   ```

3. **Dependencies**
   ```bash
   brew install espeak-ng
   ```

4. **Configuration**
   Add to `.env.local`:
   ```
   PIPER_PATH=/path/to/piper/build/piper
   PIPER_MODEL_PATH=/path/to/piper/models/en_US-libritts-high.onnx
   ```

## 🔐 Google Integration

### OAuth Setup
1. **Google Cloud Console**
   - Create/select project
   - Enable APIs
   - Generate credentials
   - Configure URIs

2. **API Permissions**
   Required scopes:
   - `https://www.googleapis.com/auth/gmail.readonly`
   - `https://www.googleapis.com/auth/calendar.events`

3. **Environment Variables**
   ```
   NEXT_PUBLIC_GOOGLE_CLIENT_ID=your_client_id
   GOOGLE_CLIENT_SECRET=your_client_secret
   ```

## 💬 Using YourAI

### Voice Commands
- **Activation**: "Hey YourAI" or "Hello"
- **Email**: "Check my health emails"
- **Appointments**: "Schedule a checkup"

## 🧠 System Architecture

### Dual-Thread Processing
1. **Text Processing**
   - AI responses
   - User input handling
   - Conversation management

2. **Audio Processing**
   - Speech recognition
   - Voice synthesis
   - Audio playback

## 🎓 Custom Voice Training

### Model Development
1. **Data Collection**: `audio_download_create_wav_files.py`
2. **Data Processing**: `process_wav_files_to_remove_wav_errors.py`
3. **Transcription**: `transcript.py` with Whisper
4. **Training**: Custom voice model creation

[Training Guide](https://colab.research.google.com/github/rmcpantoja/piper/blob/master/notebooks/piper_multilingual_training_notebook.ipynb)

## 💻 Development

```bash
npm run dev
```

## 🤝 Contributing

Join our mission to transform healthcare:

1. Fork the repository
2. Create feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open Pull Request

## 🌟 About YourAI

YourAI represents a paradigm shift in healthcare technology. Our mission is to empower healthcare professionals and patients alike through advanced AI capabilities. By analyzing vast amounts of health data and extracting meaningful insights, we're revolutionizing personal health record management.

### Impact Areas
- **Data Centralization**: Unified health records
- **Insurance Optimization**: Streamlined processes
- **Medication Management**: Enhanced administration
- **Personalized Care**: Custom health guidance
- **Privacy Protection**: Advanced security measures
- **Hospital Integration**: Seamless communication
- **Insurance Interface**: User-friendly management
- **Secure Access**: Protected data handling
- **Health Monitoring**: Continuous tracking

### Project Origins
Developed during the Princeton University Hackathon, YourAI emerged from a team of three innovators dedicated to solving healthcare challenges. Our solution combines cutting-edge technology with user-centric design to make healthcare more accessible.

### Technical Excellence
Built on React and Node.js, YourAI implements robust security measures and efficient data handling protocols, ensuring the highest standards of privacy and performance.

### Future Roadmap
- **Technology Integration**: Emerging tech adoption
- **UX Enhancement**: Improved user experience
- **Solution Expansion**: Broader health services
- **AI Advancement**: Enhanced capabilities
- **Security Reinforcement**: Stronger protection

---

<div align="center">
  <h3>Join the Healthcare Revolution</h3>
  <p>YourAI is transforming healthcare, one interaction at a time.</p>
</div>
