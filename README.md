# Read My Lips

## Overview

Read My Lips is a project aimed at revolutionizing communication for individuals with hearing impairments, deafness, and speech challenges. Leveraging cutting-edge machine learning and computer vision techniques, this system interprets the lips movement of a person from video inputs, converts it to text, and generates lifelike speech using advanced Text-to-Speech (TTS) technology.

## Table of Contents

- [Usage](#usage)
- [Project Structure](#project-structure)
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
