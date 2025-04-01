# Communication Analysis Tool for Human-AI Interaction Driving Simulator Experiments – Screening Test
# AI Communication Analyzer

Demo video - https://drive.google.com/drive/folders/1VxsCozuMETYCC6aeIo4wjCrtwoLM6nsE?usp=sharing
An AI-powered tool that analyzes audio files, transcribes speech, and provides sentiment analysis on the transcribed content.

## Features

- Audio file processing with 5-second chunking
- Speech transcription using OpenAI's Whisper model
- Sentiment analysis using NLTK's VADER
- Interactive visualizations with Plotly
- Downloadable CSV results
- Automatic FFmpeg detection and installation

## Requirements

- Python 3.8+
- FFmpeg (auto-installable from the application)

## Installation

1. Clone this repository:
```
git clone https://github.com/dhanushgithubrepo/Communication-Analysis-Tool-for-Human-AI-Interaction-Driving-Simulator-Experiments-Screening-Test.git
cd app.py
```

2. Install the required packages:
```
pip install -r app-requirements.txt
```

3. Download NLTK data (optional, will be downloaded automatically on first run):
```
python -c "import nltk; nltk.download('vader_lexicon')"
```

## Usage

1. Run the Streamlit app:
```
streamlit run app.py
```

2. Open your browser at http://localhost:8501

3. Upload an audio file (.wav or .mp3)

4. Click "Start Analysis" to process the audio

5. View the transcriptions, sentiment analysis, and visualizations in the respective tabs

6. Download the CSV file with the analysis results

## How It Works

1. The application splits the uploaded audio into 5-second chunks
2. Each chunk is transcribed using OpenAI's Whisper model
3. The transcriptions are analyzed for sentiment using NLTK's VADER
4. Results are displayed with interactive visualizations and can be downloaded as a CSV file

## Note About FFmpeg

The application requires FFmpeg for audio processing. If FFmpeg is not detected on your system:

1. The app will show an "Install FFmpeg" button in the sidebar
2. Clicking this button will download and set up FFmpeg automatically
3. For permanent installation, follow the instructions provided after installation

## Error Handling

The application includes robust error handling for:
- Missing dependencies
- Audio processing issues
- Transcription failures


---

## 📌 Description
This repository contains two Python programs developed to analyze communication data within simulated environments. The goal is to process audio-visual data to extract transcriptions, perform sentiment analysis, and visualize group communication dynamics.

---

## 🛠️ Features
1. **Speech-to-Text Conversion** (using OpenAI Whisper)
2. **Audio Segmentation** (chunks of 5 seconds)
3. **Sentiment Analysis** (custom pre-trained transformer-based model)
4. **Timestamp Mapping**
5. **CSV Export using pandas**
6. **Visualization of Transcriptions and Sentiments**

All the documentation on how the code works are given above the code and its relevant outputs are mentioned below each cell
