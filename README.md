# Tamil-Speech-Transcriptor

An advanced speech-to-text transcription tool focused on transcribing Tamil audio files into text. This tool leverages the `vasista22/whisper-tamil-medium` model, a fine-tuned version of OpenAI's Whisper ASR model optimized for Tamil. It can transcribe uploaded audio files or real-time audio recorded through a microphone and can run with GPU acceleration (CUDA) if available.

## Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Model Details](#model-details)
- [Acknowledgements](#acknowledgements)

---

## Project Overview

This project aims to provide a robust solution for transcribing Tamil audio to text. It’s designed for researchers, developers, or anyone interested in Tamil Automatic Speech Recognition (ASR). The application includes a Streamlit-based web interface for ease of use, allowing users to:
- Upload `.wav` audio files for transcription
- Use a microphone for live recording and transcription

This transcription tool is built on top of [Hugging Face's Transformers library](https://huggingface.co/), specifically the Whisper model, fine-tuned on extensive Tamil datasets.

---

## Features

- **Supports Batch and Real-time Transcription**: Upload `.wav` files or record via a microphone.
- **High Accuracy**: Built with a model trained on diverse Tamil ASR datasets.
- **CUDA Support**: Automatically detects and uses GPU if available, falling back to CPU if not.
- **Web Interface**: Simple and user-friendly Streamlit app for ease of access.

---

## Installation

### Prerequisites

- **Python**: Ensure Python 3.8 or higher is installed.
- **CUDA (Optional)**: If using a GPU, [install CUDA](https://developer.nvidia.com/cuda-downloads) for GPU acceleration.

### Steps

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/tamil-speech-to-text.git
   cd tamil-speech-to-text
2. **Set Up a Virtual Environment**:

python -m venv whisper-tamil
On Windows, use `whisper-tamil\Scripts\activate`

## Install Dependencies

pip install -r requirements.txt

## Download Model and Configure CUDA:
 Ensure that PyTorch and transformers are installed correctly with GPU support if applicable.

## Model Details
Model Card for [htvasista22/whisper-tamil-medium](https://huggingface.co/vasista22/whisper-tamil-medium)
This project utilizes the vasista22/whisper-tamil-medium model, specifically fine-tuned for Tamil ASR tasks.

Training Data:

IISc-MILE Tamil ASR Corpus
ULCA ASR Corpus
Shrutilipi ASR Corpus
Microsoft Speech Corpus (Indian Languages)
Google/Fleurs Train+Dev set
Babel ASR Corpus
Evaluation Data:

Microsoft Speech Corpus (Indian Languages) Test Set
Google/Fleurs Test Set
IISc-MILE Test Set
Babel Test Set

## Acknowledgements
This project and model were developed with support from the Speech Lab at IIT Madras and funded by the Bhashini: National Language Translation Mission under the Ministry of Electronics and Information Technology (MeitY), Government of India.

## License
This project is licensed under the Apache-2.0 License.

