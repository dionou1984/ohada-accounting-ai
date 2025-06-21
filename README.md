# 📊 OHADA Accounting AI

**IA de comptabilité automatisée pour les normes OHADA**  
*Reconnaissance de factures • Classification comptable • Vérification de conformité*

[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/)
[![Streamlit](https://img.shields.io/badge/UI-Streamlit-FF4B4B)](https://streamlit.io/)

## 🌟 Fonctionnalités
- **OCR intelligent** : Extraction des données depuis factures/reçus (Tesseract)
- **Classification automatique** selon le plan comptable OHADA
- **Vérification en temps réel** des règles OHADA (amortissements, seuils)
- **Génération d'écritures** compatibles SAGE/CIEL
- **Interface intuitive** (Streamlit)

## 🚀 Structure du Projet
```bash
ohada-accounting-ai/
├── .github/
│   └── workflows/
│       └── ci.yml          # Intégration continue (tests automatisés)
│
├── app/
│   ├── core/               # Cœur métier
│   │   ├── ocr.py          # Traitement des images (OpenCV + Tesseract)
│   │   ├── classifier.py   # Modèle ML de classification
│   │   └── compliance.py   # Moteur de règles OHADA
│   │
│   ├── data/               # Données de référence
│   │   ├── plan_comptable_ohada.csv
│   │   └── sample_data/    # Factures d'exemple
│   │
│   └── interface.py        # Application Streamlit
│
├── tests/                  # Tests unitaires
│   ├── test_ocr.py
│   └── test_compliance.py
│
├── docs/                   # Documentation technique
│   ├── api.md              # Spécifications techniques
│   └── ohada_rules.md      # Référence des normes
│
├── Dockerfile              # Configuration pour conteneurisation
├── requirements.txt        # Dépendances principales
└── LICENSE
