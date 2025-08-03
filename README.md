# **Meeting-Minutes**
# AI Meeting Minutes Generator

## Overview

An intelligent meeting transcription and analysis system that automatically converts audio recordings into professional, structured meeting minutes with comprehensive action item extraction and data analysis capabilities.

---

## Features

### Core Functionality

- **High-Accuracy Transcription**: Leverages OpenAI Whisper API for speech-to-text conversion with 95% accuracy  
- **Intelligent Content Analysis**: Utilizes Meta Llama 3.1 8B model for structured content generation  
- **Automated Data Extraction**: Identifies and extracts emails, dates, times, and action items using advanced pattern recognition  
- **Multi-Format Support**: Optimized templates for General, Project, and Executive meeting types  
- **Professional Output**: Generates clean, structured markdown documentation ready for distribution  

### Technical Capabilities

- **Memory Optimization**: 4-bit quantization reduces GPU memory requirements from 16GB to 4GB  
- **Real-Time Processing**: Progress tracking and status updates throughout the transcription pipeline  
- **Interactive Web Interface**: User-friendly Gradio interface with drag-and-drop functionality  
- **Structured Data Export**: JSON format extraction of key meeting elements for further processing  

---

## Architecture

> **Pipeline**:  
`Audio Input → Whisper Transcription → Data Extraction → Llama Processing → Structured Output`

### Key Components

- `MeetingMinutesGenerator`: Core processing class handling transcription and analysis  
- `Structured Data Extractor`: Regex-based pattern matching for information identification  
- `Template Engine`: Dynamic prompt generation based on meeting type  
- `Web Interface`: Gradio-based frontend for user interaction  

---

## Technical Specifications

### Models Used

- **Transcription Model**: OpenAI Whisper-1  
- **Language Model**: Meta Llama 3.1 8B Instruct  
- **Quantization**: 4-bit BitsAndBytes configuration with NF4 optimization  

### System Requirements

- Python 3.8 or higher  
- CUDA-compatible GPU (T4 or better recommended)  
- 8GB+ system RAM  
- OpenAI API access  
- HuggingFace account with model access  

---

## Installation

### Prerequisites

- Ensure GPU runtime is enabled  
- Obtain OpenAI API key with Whisper access  
- Create HuggingFace account and generate access token  

### Setup Instructions

```bash
git clone https://github.com/yourusername/Meeting-Minutes-.git
cd Meeting-Minutes-
