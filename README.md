# Industrialized Ostracism Hypothesis (IOH) - Simulation Model

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This repository contains the computational simulation and data visualization code for the empirical analysis section of the paper: **"Industrialized Ostracism: How Digital Platforms Weaponize the Tribal Brain Against Authentic Self-Expression."**

## Overview
The Industrialized Ostracism Hypothesis (IOH) proposes that engagement-maximizing algorithms systematically convert linear human moral-emotional expression into exponential social punishment (ostracism signals). 

This repository provides a reproducible Monte Carlo simulation that models the interaction between human behavioral inputs (moral intensity) and algorithmic amplification. The script generates an environment of $N = 10,000$ expressions to visualize the resulting threat curve: $E_{threat}^{digital} \gg E_{threat}^{ancestral}$.

## Repository Contents
* `IOH_Data_Analysis.ipynb`: The primary Jupyter/Colab notebook containing the simulation parameters, algorithmic multiplier logic, and plotting functions.
* `fig1.png`: The generated publication-ready scatterplot demonstrating the exponential scaling of the ostracism ratio.

## Dependencies
The simulation is built in Python and requires the following libraries:
* `numpy` (Statistical distributions and mathematical modeling)
* `pandas` (Dataframe manipulation)
* `matplotlib` & `seaborn` (High-resolution data visualization)

## How to Run
The environment is optimized for Google Colab to ensure zero-friction reproducibility.
1. Open `IOH_Data_Analysis.ipynb` in GitHub.
2. Click the **"Open in Colab"** badge at the top of the notebook (or download the `.ipynb` file and upload it to your Colab environment).
3. Run all cells to reproduce the dataset and the Fig 1 exponential threat curve.

## Methodology Note
To ensure scientific reproducibility, the random seed (`np.random.seed(42)`) is hardcoded into the simulation. The model relies on a log-normal distribution for baseline engagement and a beta distribution for moral intensity, mirroring empirically observed distributions on major social networks.

## License
This project is licensed under the MIT License - see the LICENSE file for details.
