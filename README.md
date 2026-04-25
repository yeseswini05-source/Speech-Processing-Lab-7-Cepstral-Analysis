#  Speech Processing Lab 7 - Cepstral Analysis

 Objective

* Perform cepstral analysis of a speech signal
* Estimate pitch frequency
* Separate excitation and vocal tract components
* Analyze signal in the quefrency domain


 Files in this Repository

* `speechProcessinglab_7(2).ipynb` → Implementation code
* `speechprocessingLab7_report.pdf` → Detailed lab report


 Important Note About Audio File

The original audio used in this experiment is **not included** due to privacy reasons.

 You must provide your own input audio file to run the code.


 How to Create the Required Audio File

 Step 1: Record Audio

* Record a short speech sample (2–5 seconds)
* Use your phone or laptop microphone



 Step 2: Convert to WAV Format

If your file is `.m4a`, convert it using FFmpeg:

```
ffmpeg -i input.m4a -ac 1 -ar 16000 speech.wav
```



 Step 3: File Requirements

Make sure your file:

* Is named **`speech.wav`**
* Is **mono (1 channel)**
* Has **sampling rate = 16000 Hz**


 Step 4: Place the File

Put `speech.wav` in the **same folder as the notebook**



 How to Run the Project

 1. Install Dependencies

```
pip install numpy matplotlib librosa scipy
```

 2. Run Notebook

```
jupyter notebook speechProcessinglab_7(2).ipynb
```



  Expected Output

* Real cepstrum plot
* Pitch detection (5–20 ms range)
* Separation of:

  * Vocal tract (low-time cepstrum)
  * Excitation source (high-time cepstrum)



 Key Concepts

* Cepstrum = IFFT(log(|FFT(x)|))
* Quefrency analysis
* Pitch estimation from cepstral peak
* Liftering for signal separation



 Results Summary

* Successfully computed real cepstrum
* Identified pitch period from cepstrum peak
* Estimated pitch frequency within normal speech range (80–300 Hz)
* Separated excitation and vocal tract components


 Author: K. Shiva Gnana Yeseswini
BL.EN.U4AIE23013


