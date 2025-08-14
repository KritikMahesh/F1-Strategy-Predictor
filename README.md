# 🏎️ F1 Strategy Predictor

[![Open In Kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/code)
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
