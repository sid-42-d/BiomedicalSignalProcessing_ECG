# Multi-Channel Biosignal Acquisition and Processing

## Overview
This project focuses on acquiring and processing multiple physiological signals using biomedical instrumentation and Python-based signal processing. The goal is to clean and analyze signals such as ECG, PPG, and Dynamometer measurements to understand their characteristics in both time and frequency domains.

## Signals Used
- **ECG (Electrocardiogram)** – cardiac electrical activity  
- **PPG (Photoplethysmography)** – blood volume changes  
- **Dynamometer** – muscle force measurement  

All signals were recorded simultaneously from human subjects in a controlled laboratory setup.

## Processing Pipeline

### 1. Data Acquisition
- Multi-channel physiological signals were recorded using biomedical instrumentation.
- Signals were sampled at **1000 Hz**.

### 2. Signal Filtering
- **50 Hz Notch Filter** used to remove powerline interference.
- **4th-order Butterworth Low-Pass Filters** applied:
  - ECG → 100 Hz cutoff  
  - PPG → 10 Hz cutoff  
  - Dynamometer → 20 Hz cutoff  

### 3. Signal Analysis
- Compared raw and filtered signals in the **time domain**.
- Performed **FFT-based frequency analysis** to evaluate filtering performance.
- Used spectral plots to verify noise removal and signal quality.

## Tools and Libraries
- Python
- NumPy
- SciPy
- Matplotlib

## Output
The project generates:
- Time-domain plots of raw vs filtered signals
- Frequency spectrum comparison before and after filtering
- Visualization of signal quality improvement after processing

## Learning Outcomes
- Practical understanding of **biosignal acquisition and preprocessing**
- Implementation of **digital filters for noise removal**
- Application of **FFT for frequency-domain analysis**
- Visualization and interpretation of physiological signals
