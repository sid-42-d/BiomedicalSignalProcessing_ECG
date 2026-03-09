# Biomedical Signal Processing – ECG Analysis

## Overview
This project focuses on the acquisition and preprocessing of multi-channel physiological signals including **ECG, PPG, and Dynamometer signals**. The signals were collected using biomedical instrumentation and processed using Python-based signal processing techniques to remove noise and analyze their characteristics in both time and frequency domains.

## Signals Used
- **ECG (Electrocardiogram)** – Electrical activity of the heart  
- **PPG (Photoplethysmography)** – Blood volume changes in tissue  
- **Dynamometer** – Muscle force measurement  

All signals were recorded simultaneously from human subjects in a controlled laboratory environment.

## Signal Processing Pipeline

### Data Acquisition
Multi-channel physiological signals were recorded and sampled at **1000 Hz**.

### Signal Filtering
To remove noise and interference:

- **50 Hz Notch Filter** used to eliminate powerline interference  
- **4th-order Butterworth Low-Pass Filters** applied:
  - ECG → 100 Hz cutoff
  - PPG → 10 Hz cutoff
  - Dynamometer → 20 Hz cutoff

### Frequency Analysis
- **Fast Fourier Transform (FFT)** used to analyze frequency components
- Comparison of **raw vs filtered ECG signals** in both time and frequency domains

## Libraries Used
- Python
- NumPy
- SciPy
- Matplotlib

## Dataset
The dataset used in this project is hosted externally due to GitHub repository size best practices.

Download the dataset here:

https://drive.google.com/file/d/1PaDHAhDhR5QUOnqH7Oq0KLn4rM2TeZnk/view?usp=sharing

After downloading, place the dataset file inside the `data/` folder before running the notebook.

## Project Structure

```
BiomedicalSignalProcessing_ECG
│
├── data
│ └── DATASET.md
│
├── notebooks
│ └── ecg_signal_filtering_analysis.ipynb
│
├── README.md

```
## Learning Outcomes
- Practical experience with **biosignal acquisition and preprocessing**
- Implementation of **digital filters for physiological signal processing**
- Application of **FFT-based frequency domain analysis**
- Visualization and interpretation of biomedical signals
