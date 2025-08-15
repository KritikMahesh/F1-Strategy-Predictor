# 🏎️ F1 Strategy Predictor

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/#scrollTo=P4HZqbKe399i&fileId=https%3A//storage.googleapis.com/kaggle-colab-exported-notebooks/kritikmahesh/f1-predictor-ipynb.49bfd94d-0b3a-4687-b3ca-f99d2fc5d4b1.ipynb%3FX-Goog-Algorithm%3DGOOG4-RSA-SHA256%26X-Goog-Credential%3Dgcp-kaggle-com%2540kaggle-161607.iam.gserviceaccount.com/20250815/auto/storage/goog4_request%26X-Goog-Date%3D20250815T131623Z%26X-Goog-Expires%3D259200%26X-Goog-SignedHeaders%3Dhost%26X-Goog-Signature%3D9b44c208bebcad55024f16e2be2c65a3ca58fae00b9bac4de89005ceda24bc0ab46a7884fd46cc10629483da4786f00123812d3282a2fafb1ca7afcd3a65ff1ef81a30e4b79582fd0f56be79b94afc0c93f70ed000fdd77bd536d4147c3700cb3d7d7e6cebc049f65158a82eb098e63bc0a82486300ac4959d33d28cf70def7bbb2b2e3cb49f2bf63d64cdd8a374a34708c7829932daf8df7c800d5a8b9c0bbf6047053122db7ae3d070483e6cf11c3d851c3fb3b2eedf26fe74b628fa49d3c12fc6f1ecc072f7db634939da1f84084a39b66642f85d0b2b7c90280668717a42f382780926d32caee42193d4eecf363bc3d6bc9123e0464b7136475d73565be3)

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![FastF1](https://img.shields.io/badge/FastF1-2.3+-red.svg)](https://theoehrly.github.io/Fast-F1/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-visualization-yellow.svg)](https://matplotlib.org/)

> **Predict and visualize Formula 1 race strategies using telemetry, simulated weather, and performance modelling in a Kaggle-ready notebook.**

This repository contains a **Jupyter Notebook** built for advanced Formula 1 strategy prediction. Leveraging [FastF1](https://theoehrly.github.io/Fast-F1/) for official timing and telemetry, it combines race history, tyre wear models, and environmental factors to project race outcomes — no API keys required.

## 📋 Table of Contents

* [About](#-about)
* [Features](#-features)
* [Architecture](#-architecture)
* [Installation](#-installation)
* [Usage](#-usage)
* [Workflow](#-workflow)
* [Example Outputs](#-example-outputs)
* [Technical Notes](#-technical-notes)

## 🎯 About

**F1 Strategy Predictor** is an interactive analysis tool where you choose a season, Grand Prix, driver, and conditions to see how strategies unfold. It integrates historical telemetry with simulated weather and pit strategies to show how races could play out.

## ✨ Features

* 📅 **Interactive Selection** — Choose season, Grand Prix, driver
* 📈 **Telemetry Insights** — Lap time, sector performance, speed traces
* 🛞 **Tyre Wear Modelling** — Estimate degradation over laps
* 🌦 **Simulated Weather** — Adjust track temperature, wind, rain probability
* 🔄 **Strategy Comparison** — Pit stop timing and compound choice scenarios
* 🏁 **Race Replay** — Simulated position changes over race distance
* 💾 **Offline Ready** — Cached data for repeat sessions

## 🏗️ Architecture

```
User Input → FastF1 Data Fetch → Pandas/Numpy Preprocessing
Interactive Widgets → Strategy Engine → Visual Outputs
```

## 🛠️ Installation

**Kaggle (Recommended)**

1. Open [Kaggle Notebooks](https://www.kaggle.com/code)
2. Create a **New Notebook**
3. Upload `f1_predictor.ipynb`
4. Run all cells in order

## 🚀 Usage

1. Choose season, Grand Prix, and driver
2. Set simulated weather and tyre strategy
3. Run the notebook for telemetry, strategy, and simulation outputs
4. Compare alternate race strategies visually

## 🔄 Workflow

1. **Acquire Data** — Load & cache GP session data
2. **Process** — Merge telemetry, pit stop, and synthetic weather
3. **User Interaction** — Configure race parameters
4. **Simulation** — Apply tyre wear models & strategy logic
5. **Visualization** — Generate plots and race replay graphs

## 📊 Example Outputs

* Lap time progression
* Tyre compound usage timelines
* Pit stop breakdowns
* Position change simulations

## 🧠 Technical Notes

* First-time data load may take several minutes
* Weather is simulated — no external API
* Clear FastF1 cache to refresh data

---

## ^.^/
  
