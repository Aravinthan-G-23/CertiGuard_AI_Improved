# CertiGuard_AI_Improved
AI-powered certificate authenticity detector using EfficientNetB3 + 3-phase fine-tuning.
Dataset

✅ Real: 169 | ❌ Fake: 121 | Total: 290

Features

Classifies certificates as Genuine / Fake / Uncertain
Auto-computes optimal threshold via F1 sweep
Test-Time Augmentation (TTA × 8) for stable predictions
OCR text extraction with Trust Score
MongoDB logging + Streamlit UI via ngrok

Quick Start
bash# Open CertiGuard_AI_Improved.ipynb in Google Colab (GPU runtime)
# Run all cells top to bottom
# Set your ngrok token in the last cell
# Get your public URL and open in browser
Model
PhaseTrained LayersLR1Head only1e-32Head + top 601e-43Full model5e-6
Results
MetricScoreAccuracy~92–95%AUC~0.96–0.98F1~0.92–0.95
Tech Stack
TensorFlow 
EfficientNetB3 
EasyOCR 
Streamlit 
MongoDB 
ngrok 
scikit-learn
Dataset Source
Real and Fake Internship Documents – Kaggle
