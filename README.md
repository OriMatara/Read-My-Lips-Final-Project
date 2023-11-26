# Read My Lips

## Overview

Read My Lips is a project aimed at revolutionizing communication for individuals with hearing impairments, deafness, and speech challenges. Leveraging cutting-edge machine learning and computer vision techniques, this system interprets the lips movement of a person from video inputs, converts it to text, and generates lifelike speech using advanced Text-to-Speech (TTS) technology.

## Table of Contents

- [Usage](#usage)
- [Project Structure](#project-structure)
- [Algorithm Overview](#algorithm-overview)
- [Results](#results)
- [Dependencies](#dependencies)
- [Acknowledgments](#acknowledgments)

## Usage

1. **Prepare Your Video Data  for Lip Reading.**

2. **Run Lip Reading and Speech Synthesis.**

3. **Evaluate the Results.**

## Project Structure

- `code/`: Main codebase for lip reading and speech synthesis.
  - `lip_reading.py`: Lip reading model implementation.
  - `speech_synthesis.py`: Text-to-Speech synthesis.
- `data/`: Dataset and relevant data.
- `models/`: Trained model storage.
- `results/`: Folder for evaluation results.
- `notebooks/`: Jupyter notebooks for exploration and analysis.

## Algorithm Overview

**Read My Lips** employs a multi-step algorithm to interpret lip movements and convert them into synthesized speech:

1. **Face and Lip Region Detection:**
   - Identify faces and extract the Region of Interest (ROI) representing the lips from input video frames.

2. **Spatial-Temporal Convolutional Neural Network (STCNN):**
   - Utilize a three-layer STCNN to recognize lip movement patterns across frames.

3. **Gated Recurrent Units (GRU) - Recurrent Neural Network (RNN) Fusion:**
   - Convert extracted elements into numerical vectors, filtering essential information using GRU and preserving sequences with LSTM.

4. **Connectionist Temporal Classification (CTC) Loss:**
   - Feed the character sequence into CTC loss to minimize errors, producing the final output of words and sentences.

5. **Text-to-Speech (TTS) Integration:**
   - Process the algorithm's text prediction output with a TTS algorithm, creating a sequence of speech sounds.

6. **Speech Synthesis and Parameter Adaptation:**
   - Generate speech amplitudes representing synthesized speech, adjusting parameters to match linguistic characteristics.

7. **IBM-Watson TTS API:**
   - Implement the TTS algorithm using IBM-Watson TTS API, leveraging an AI-based system for efficient speech synthesis.

The results are written sentence and synthesized speech output reflecting the lip movements captured in the input video.

## Results

### Character Error Rate (CER): 7%
### Word Error Rate (WER): 12%

## Dependencies

- TensorFlow 2.10
- IBM Watson Text-to-Speech
- Other dependencies listed in `requirements.txt`

## Acknowledgments

- Special thanks to [IBM Watson](https://www.ibm.com/watson) for providing Text-to-Speech services.
- The dataset used in this project is based on the GRID dataset.

Feel free to contribute or report issues!
