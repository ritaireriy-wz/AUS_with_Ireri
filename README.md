# AUS_with_Ireri
Learn and Implement AUS theories with me
Computer Science for Autonomous Systems: NumPy Weather & Signal Processing Analysis

A repository containing vectorized Python implementations, data analysis exercises, and theoretical notes for the Computer Science for Autonomous Systems (MSc) curriculum at ELTE.

📌 Project Overview

This repository focuses on high-performance data manipulation and mathematical analysis using NumPy. It explores two primary domains:

Weather Data Analysis (Almaty Dataset):

Vectorized operations on 12-month climate data 

Calculation of ecological and climate metrics such as the De Martonne Aridity Index.

Season-based indexing, masked array filtering, copy-overwrite logic, and conditional aggregation.

Signals, Systems, and Sampling Foundations:

Discrete and Continuous Linear Time-Invariant (LTI) systems.

Transfer functions and Butterworth / RC circuit low-pass filters.

Uniform sampling, Nyquist–Shannon theorem, and aliasing effect analysis.

Key NumPy Techniques & Concepts

Vectorized Operations: Executing element-wise arithmetic, mathematical transformations (e.g., Celsius to Fahrenheit), and comparisons without explicit Python for loops.

1-Based vs. 0-Based Month Indexing: Standardizing seasonal bounds (e.g., Spring slicing [2:5] for March–May) and converting argmax indices to calendar month numbers ($1\text{-based index} = \text{array index} + 1$).

Fancy & Boolean Indexing: Filtering arrays using positional index lists (e.g., temperatures[[11, 0, 1]] for winter months) or bitwise mask combinations (&, |, ~).

Array Copying & Suppression: Utilizing np.ndarray.copy() alongside non-target value suppression (-np.inf) to extract sub-sequence extrema safely without mutating source data.

Type Casting: Converting NumPy scalar primitives (np.float32, np.bool_, np.int64) to standard Python types (float, bool, int) for serialization and strict autograder compatibility.

📂 Repository Structure

.
├── notebooks/
│   └── weather_analysis.ipynb   # Interactive Jupyter notebook with exercises
├── src/
│   ├── weather_analytics.py     # Clean Python functions for seasonal & climate metrics
│   └── signal_processing.py     # Signal sampling and discrete filter implementations
├── README.md                    # Project documentation
└── requirements.txt             # Dependency specifications
