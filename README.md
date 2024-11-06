# TI FMCW Radar Simulation and Parameter Estimation Tools

This repository contains a series of Jupyter notebooks for simulating and understanding the Texas Instruments FMCW radar system, specifically focusing on AWR boards. These notebooks serve both pedagogical and practical purposes, from learning key radar concepts to calculating essential parameters for radar configuration.

## FMCW Radar Overview

Frequency-Modulated Continuous Wave (FMCW) radars work by transmitting a signal that continuously varies in frequency over a specific range. When this signal reflects off a target, the radar measures the frequency difference between the transmitted and received signals. This difference, known as the beat frequency, is directly related to the distance to the target. By analyzing changes in beat frequency over time, the radar can also determine the relative velocity of moving targets. FMCW radar is widely used for applications requiring precise distance and speed measurements, such as automotive sensing and industrial monitoring.

## Overview of Notebooks

1. **Doppler Simulation.ipynb**
   - This notebook provides a simulated environment to understand how Doppler frequency changes can influence the behavior of an FMCW radar system. It is designed to enhance comprehension of the underlying principles of velocity and distance detection in radar systems.
   - **Key Learning Goals:**
     - Gain insight into how radar signals are influenced by the Doppler effect.
     - Understand the relationship between signal sampling rate and resolution in velocity and distance measurements.

2. **exercises FFT.ipynb**
   - A focused exercise notebook on Fast Fourier Transform (FFT), highlighting how different sampling rates affect resolution. Understanding this concept is crucial to adjusting the radar's parameters for desired velocity and distance resolutions.
   - **Key Learning Goals:**
     - Explore the impact of sampling rate (sampling frequency) on FFT resolution.
     - Connect sampling rate choices with changes in velocity and distance resolution in radar data analysis.

3. **parameters_estimators.ipynb**
   - This practical notebook calculates the required input parameters for configuring AWR radar boards based on desired operational specifications. It considers target resolution, maximum detectable velocity, and distance, translating these needs into specific radar configuration values.
   - **Key Features:**
     - Input necessary for AWR radar configuration based on resolution and operational range requirements.
     - Provides parameter calculations tailored for TI AWR boards, aiding in accurate and efficient radar configuration.

4. **From-Parameters-Chirp-Simulation.ipynb**
   - Using configuration data from TI's default SDK, this notebook simulates the theoretical behavior of the radar system. The simulation is organized in a class-based structure, which improves readability and usability. Each parameter used in the simulation is explained within the code comments for clarity.
   - **Key Features:**
     - Class-oriented code structure for easy customization and reusability.
     - Simulates radar behavior using TI SDK configuration files, providing insights into how specific settings affect radar operation.

## Parameter Descriptions

Each notebook contains inline comments explaining parameter choices and calculations. In particular, `From-Parameters-Chirp-Simulation.ipynb` includes detailed explanations for each radar parameter to help users understand the simulation's behavior and outcomes.
