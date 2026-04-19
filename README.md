# Side-Channel Attacks - Team_no_1

This project implements a **Side-Channel Attack (SCA)** on the Advanced Encryption Standard (AES) to recover the 16-byte secret key from the power consumption traces. 
It shows how cryptographic implementations can leak sensitive information through physical side channels even when the underlying algorithm is secure.

---

## Features
- Hamming Weight–based modelling of intermediate AES computations  
- Correlation between predicted and real power traces  
- Visualisation of correlation peaks for key identification
- Byte-wise key recovery across all 16 key bytes  
- End-to-end verification using AES decryption  

---


## Project Structure
SC4015/
├── SC4015_SCA_Team_no_1.ipynb
├── waveform.csv
└── results/
    ├── plots/                 # Per-byte correlation graphs
    └── analysis_summary.csv   # Key bytes + correlation strengths



## How to Run

1. Open the notebook SC4015_SCA_Team_no_1.ipynb in **Google Colab**  
2. Mount Google Drive:
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   

## Results
- Recovered the complete AES-128 secret key  
- Verified correctness by decrypting ciphertext back to the original plaintext  
- Clear correlation peaks observed for correct key candidates across all bytes  

---

### Result Directory

The notebook automatically creates the following directory:

/content/drive/My Drive/Colab Notebooks/SC4015/results/

This directory contains:
- results/plots/ → per-byte CPA analysis visualisations  
- results/analysis_summary.csv → recovered key and correlation values


