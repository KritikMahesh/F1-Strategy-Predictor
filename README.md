# 🏎️ F1 Strategy Predictor

[![Open In Kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/code)
[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![FastF1](https://img.shields.io/badge/FastF1-2.3+-red.svg)](https://theoehrly.github.io/Fast-F1/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-visualization-yellow.svg)](https://matplotlib.org/)

> **Predict, analyze, and visualize Formula 1 race strategies using historical telemetry, simulated weather, and performance modelling — all in one Kaggle-ready notebook.**

This repository contains a Jupyter Notebook for advanced **Formula 1 strategy analysis and prediction**. Using [FastF1](https://theoehrly.github.io/Fast-F1/) data, it enables deep telemetry exploration, tyre degradation modelling, pit stop simulations, and multi-factor outcome projections without needing any API keys.

---

## 📋 Table of Contents

* [About](#-about)
* [Features](#-features)
* [Architecture](#-architecture)
* [Installation](#-installation)
* [Usage](#-usage)
* [Workflow](#-workflow)
* [Example Outputs](#-example-outputs)
* [Technical Notes](#-technical-notes)

---

## 🎯 About

The **F1 Strategy Predictor** simulates race strategies by combining historical telemetry with user-selected parameters such as Grand Prix location, driver, weather conditions, and tyre strategy. The result is an interactive and visual approach to understanding competitive decision-making in F1.

---

## ✨ Features

* 📅 **Interactive Parameter Selection** — Year → Grand Prix → Session → Driver
* 📈 **High-Resolution Telemetry Analysis** — Lap time trends, sector splits, speed traces
* 🛞 **Tyre Degradation Modelling** — Regression-based wear estimation
* 🌦 **Simulated Weather Adjustments** — Temperature, wind, rain probability
* 🔄 **Strategy Comparison Mode** — Pit stop timing & tyre choice simulations
* 🏁 **Race Replay Projection** — Simulated position changes throughout the race
* 💾 **Offline Cache** — FastF1 SQLite caching for re-runs without internet

---

## 🏗️ Architecture

```
User Input → FastF1 Data Fetch → Pandas/Numpy Preprocessing
Widgets & Controls → Matplotlib/Plotly Visuals
Weather Simulation → Strategy Model Engine → Analysis Outputs
```

---

## 🛠️ Installation

### Kaggle (Recommended)

1. Go to [Kaggle Notebooks](https://www.kaggle.com/code)
2. Start a **New Notebook**
3. Upload `f1_predictor.ipynb`
4. Run cells sequentially to interact with the strategy predictor

---

## 🚀 Usage

1. Select **season**, **Grand Prix**, and **driver**
2. Adjust simulated **weather** and **tyre strategy**
3. Run analysis to get telemetry graphs, tyre usage charts, and position simulations
4. Compare different strategies to see possible race outcomes

---

## 🔄 Workflow

1. **Data Acquisition** — Load & cache session data via FastF1
2. **Processing** — Merge lap telemetry, weather simulation, pit stop data
3. **Interaction** — User sets race parameters
4. **Computation** — Model degradation & simulate results
5. **Visualization** — Output strategy charts and replay graphs

---

## 📊 Example Outputs

* **Lap Time Trends** — Driver pace evolution
* **Tyre Strategy Charts** — Compound usage and change points
* **Pit Stop Analysis** — Tabular + visual breakdown
* **Race Position Simulation** — Projected position changes over laps

---

## 🧠 Technical Notes

* Initial data load may take a few minutes for new GP sessions
* Weather simulation is synthetic, no external API used
* Clear FastF1 cache to refresh data
