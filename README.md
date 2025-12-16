# OpenAI Transcribe Tester

A modern, beautiful UI for testing OpenAI's Speech-to-Text API.

## Features

- **Model Selection**: Choose between whisper-1, gpt-4o-transcribe, gpt-4o-mini-transcribe, and gpt-4o-transcribe-diarize
- **Audio Recording**: Record audio directly from your microphone with real-time waveform visualization
- **File Upload**: Upload audio files (MP3, WAV, M4A, etc.) or video files (MP4, WebM)
- **Audio Extraction**: Automatically extracts audio from video files using [Mediabunny](https://github.com/vanilagy/mediabunny)
- **Diarization Support**: View speaker-segmented transcripts with the diarize model
- **Multiple Output Formats**: JSON, text, SRT, VTT, verbose JSON, and diarized JSON

## Usage

1. Open `index.html` in a browser (or serve with a local server)
2. Enter your OpenAI API key
3. Select a transcription model
4. Either record audio or upload a file
5. Click "Transcribe Audio"

## Supported File Types

- Audio: MP3, WAV, M4A, MPEG, MPGA, OGG, WebM
- Video: MP4, WebM (audio will be extracted automatically)

## Running Locally

```bash
# Using Python
python3 -m http.server 8080

# Using Node.js
npx serve .
```

Then open http://localhost:8080

## Tech Stack

- Vanilla JavaScript (ES Modules)
- [Mediabunny](https://github.com/vanilagy/mediabunny) for audio extraction from video
- Web Audio API for recording and visualization
- OpenAI Audio Transcriptions API

