# ISS Project 2025/26 – Music Search (MIR)

This repository contains a solution to the **ISS (Signals and Systems)** course project at **FIT VUT**, focused on a basic **Music Information Retrieval (MIR)** task similar to applications such as Shazam.

📌 Project Description

The goal of the project is to identify short unknown audio clips by comparing them to a database of known audio signals.  
The task is formulated as a similarity search problem over audio features extracted from WAV files.

- Known audio clips: 706 × 10 s
- Unknown audio clips: 50 × 5 s
- Sampling rate: 16 kHz, mono WAV

The output of the solution is a **similarity matrix** of size `50 × 706`, where higher values indicate higher similarity between unknown and known signals.

🧠 Approach

The solution is based on classical digital signal processing techniques:

- Short-time analysis of audio signals
- Spectrogram-based feature extraction (amplitude spectrum)
- Normalization to reduce the influence of filtering and noise
- Similarity computation using correlation / matched filtering–like methods

No specialized MIR libraries or cloud-based services are used, in accordance with the assignment requirements.

The focus of the project is **understanding the signal processing pipeline**, not achieving perfect classification accuracy.

🛠️ Implementation

- Language: Python (Jupyter Notebook)
- Input: WAV audio files
- Output: similarity matrix and `eval.txt` file for scoring
- Evaluation performed using the provided validation and scoring scripts

The implementation is designed to be runnable on standard Linux/Windows environments or Google Colab.

📊 Results

The implemented method was evaluated on the provided validation dataset.  
Top-1 and Top-5 accuracy metrics were used to assess performance, and multiple approaches were compared during development.

Details, figures, and analysis are documented in the accompanying project report.

🎓 Context

This project was developed as part of the **ISS – Signály a systémy** course at **Brno University of Technology (FIT VUT)** during the academic year 2025/26.

