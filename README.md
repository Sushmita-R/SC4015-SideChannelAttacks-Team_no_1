# AES Correlation Power Analysis (CPA)

This project demonstrates a Correlation Power Analysis (CPA) attack on AES to recover the 16-byte secret key using power traces.

## Key Features
- Hamming Weight leakage model
- Byte-wise key recovery (0–15)
- Correlation analysis across 256 key guesses
- Visualization of correlation peaks
- Key verification using AES decryption

## Results
- Successfully recovered AES-128 key
- Verified using ciphertext decryption

## Files
- `SC4015_Lab_2_v2.ipynb` – Main notebook
- `waveform.csv` – Power traces
- `plots/` – Per-byte correlation graphs

## How to Run
1. Open in Google Colab
2. Mount Google Drive
3. Run all cells

## Technologies Used
- Python
- NumPy
- Matplotlib
- PyCryptodome
