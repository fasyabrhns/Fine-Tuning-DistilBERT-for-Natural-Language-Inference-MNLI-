MUhammad Farhan 

Fasya Burhanis Syauqi

#  MultiNLI: Natural Language Inference (NLI)

![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-2.0%2B-orange)
![HuggingFace](https://img.shields.io/badge/Transformers-4.30%2B-yellow)
![Task](https://img.shields.io/badge/Task-Sentence--Pair-green)

Proyek ini berfokus pada tugas **Natural Language Inference (NLI)**, di mana model harus menentukan hubungan logika antara dua kalimat: *Premise* (Premis) dan *Hypothesis* (Hipotesis).

Model **DistilBERT** dilatih untuk memahami konteks semantik antar kalimat tersebut.

##  Tentang Dataset
Dataset yang digunakan adalah **GLUE - MNLI** (Multi-Genre NLI). Dataset ini menguji kemampuan model dalam memahami implikasi, kontradiksi, atau kenetralan.

| Label | Arti | Deskripsi |
|-------|------|-----------|
| **0** | ✅ Entailment | Hipotesis **benar** berdasarkan premis. |
| **1** | 😐 Neutral | Hipotesis **tidak berhubungan** langsung dengan premis. |
| **2** | ❌ Contradiction | Hipotesis **bertentangan** dengan premis. |

##  Struktur Proyek
```text
project_multinli/
├── notebooks/
│   └── Task3_MultiNLI.ipynb     # Notebook Training Sentence Pair
├── reports/
│   └── report.md                # Laporan Evaluasi
├── requirements.txt             # Dependencies
└── README.md                    # Dokumentasi
