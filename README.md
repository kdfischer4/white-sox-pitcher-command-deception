# White Sox Pitcher Command & Deception

## Overview

This repository highlights my capstone project for the University of Chicago's Master of Science in Applied Data Science program, completed in collaboration with the Chicago White Sox.

The objective of the project was to develop data-driven methods for quantifying two difficult-to-measure pitching attributes—**command** and **deception**—using biomechanical and pitch outcome data from the 2024 MLB season. These metrics can help baseball organizations identify undervalued pitchers and improve player development by better understanding how pitching mechanics influence on-field performance.

---

## Project Goals

The project focused on three primary objectives:

- Develop meaningful metrics for pitcher command and deception using pitch outcome data.

- Build machine learning models capable of predicting these metrics from biomechanical measurements.

- Identify which aspects of a pitcher's mechanics contribute most to command and deception, providing actionable insights for scouting and coaching.

---

## Data

The analysis combined multiple datasets provided by the Chicago White Sox and collected through MLB Hawk-Eye tracking systems, including:

- Approximately **600,000** pitches of full-body biomechanical measurements

- Approximately **700,000** pitch outcome records

- Additional hitter timing, contact quality, and expected slugging metrics

After merging the datasets, removing incomplete observations, and performing data cleaning and feature engineering, the final modeling dataset contained approximately **400,000** pitches.

---

## Approach

Our team explored several machine learning approaches to quantify command and deception and to understand the relationship between pitching mechanics and game outcomes.

Key techniques included:

- Feature engineering from biomechanical and pitch outcome data

- Gaussian Mixture Models (GMMs) for command modeling

- XGBoost models for developing command and deception metrics

- Graph Neural Networks (GNNs) to model the relationships between body joints throughout the pitching motion and identify biomechanical factors associated with deception

Rather than focusing solely on predictive performance, the project emphasized model interpretability so the resulting insights could be used by coaches and analysts.

---

## Results

The project produced several meaningful findings for the Chicago White Sox:

- Developed new command and deception metrics that improved upon the organization's existing evaluation methods.

- Graph Neural Network models achieved an **R² of approximately 0.17** when predicting deception from biomechanics alone, demonstrating a meaningful relationship despite the inherent noise in pitch-level data.

- Pitcher-level command models achieved an **AUC greater than 0.80**, identifying biomechanical characteristics associated with strong command.

- Identified key biomechanical indicators of deception, particularly involving upper-body posture and timing during the pitching delivery.

- Demonstrated that pitchers with stronger command and deception metrics consistently produced better run prevention than similarly skilled pitchers, with analysis suggesting improvements could translate to approximately **0.7 fewer runs allowed per game** and roughly **11 additional wins** under the study's assumptions.

- Awarded **Best in Show** at the University of Chicago MS in Applied Data Science Capstone Showcase.

---

## My Contributions

My primary responsibilities on the project included:

- Cleaning and preprocessing over **400,000** rows of biomechanical and pitch outcome data

- Performing feature engineering to prepare data for modeling

- Contributing to the development of command and deception scoring models using Gaussian Mixture Models and XGBoost

- Designing and implementing Graph Neural Network models to identify which biomechanical features—and at which stages of the pitching delivery—most strongly influence deception

- Interpreting model outputs and communicating findings during the final client presentation

---

## Technologies

**Programming**

- Python

**Libraries**

- Pandas

- NumPy

- Scikit-learn

- PyTorch

- PyTorch Geometric

**Machine Learning**

- Linear Regression

- Gaussian Mixture Models (GMMs)

- XGBoost

- Graph Neural Networks (GNNs)
