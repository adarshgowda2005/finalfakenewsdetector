# 📰 NewsVeracity AI - Fake News Detection System

A modern web application that uses AI to detect fake news articles. Built with Flask, Ollama, and a responsive web interface.

## 🚀 Quick Start

### Prerequisites
- Python 3.8 or higher
- Ollama installed on your system
- At least 4GB RAM (8GB recommended)

### Step-by-Step Installation

1. **Install Ollama**
   - Download from: https://ollama.com/
   - Follow the installation instructions for your operating system

2. **Extract the Project**
   ```bash
   unzip ollamamodel.zip
   cd ollamamodel
   ```

3. **Set up Python Environment**
   ```bash
   # Create virtual environment
   python -m venv venv
   
   # Activate virtual environment
   # On Windows:
   venv\Scripts\activate
   # On Mac/Linux:
   source venv/bin/activate
   ```

4. **Download AI Model**
   ```bash
   ollama pull phi3.5
   ```

5. **Install Python Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

6. **Run the Application**
   ```bash
   python app.py
   ```

7. **Access the Application**
   - Open your browser and go to: `http://localhost:5000`
   - Start analyzing news articles!

## 🛠️ Features

- **URL Analysis**: Paste news article URLs for instant verification
- **Text Analysis**: Directly input news text for detection
- **Modern UI**: Clean, responsive design that works on all devices
- **Real-time Results**: Get instant verdicts with confidence scores
- **Local Processing**: All AI processing happens locally on your machine

## 📁 Project Structure

```
ollamamodel/
├── app.py                 # Main Flask application
├── requirements.txt       # Python dependencies
├── static/
│   ├── css/
│   │   └── style.css     # Styling files
│   └── js/
│       └── script.js     # Frontend JavaScript
└── templates/
    └── index.html        # Main web interface
```

## 🔧 Troubleshooting

### Common Issues

1. **"Ollama API error: 404"**
   - Make sure Ollama is running: `ollama serve`
   - Verify the model is downloaded: `ollama list`

2. **"Analysis Failed"**
   - Check your internet connection for URL analysis
   - Ensure the news text is at least 50 characters

3. **Port already in use**
   - Change the port in `app.py`: `app.run(port=5001)`

### Verifying Installation

Check if everything is working:
```bash
# Check Ollama
ollama list

# Check Python dependencies
pip list

# Test the application
python app.py
```

## 🤖 Supported Models

- `phi3.5:latest` (Recommended)
- `gemma3:1b`
- Other Ollama models can be configured in `app.py`

## 📝 Usage Examples

1. **URL Analysis**: Paste a news article URL and click "Analyze URL"
2. **Text Analysis**: Switch to "Paste Text" tab, enter news content, and click "Analyze Text"

## ⚠️ Disclaimer

This tool provides AI-based analysis and should be used as a supplementary fact-checking aid. Always verify important information through multiple reliable sources.

## 🐛 Reporting Issues

If you encounter any problems:
1. Check the troubleshooting section above
2. Ensure all installation steps were followed correctly
3. Check that Ollama is running and the model is downloaded

---

**Note**: The application runs entirely on your local machine - no data is sent to external servers for analysis.
