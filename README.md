# TRACK2-SAU

# Carbon Emissions & Electricity Generation Analysis (2023)
This project visualizes global carbon emissions (2023) and long-term energy generation trends for Saudi Arabia & the UK using Python. It includes bar charts, bubble charts, dual-axis line charts, and stacked area charts.

## 📋 Table of Contents
1. [Project Overview](#1-project-overview)
2. [Dependencies](#2-dependencies)
3. [Data Setup](#3-data-setup)
4. [How to Run the Code](#4-how-to-run-the-code)
5. [Output Description](#5-output-description)
6. [Notes](#6-notes)

## 1. Project Overview
This code generates 8 visualizations focused on:
- Top 20 countries' total CO₂ emissions (2023)
- CO₂ emissions vs. population vs. GDP (bubble charts)
- Saudi Arabia's long-term CO₂ emissions (total/intensity)
- Saudi Arabia & UK electricity generation by source (1980–2023)

All charts use consistent styling and 2023 as the target analysis year.

## 2. Dependencies
The code requires Python and the following libraries:
- `matplotlib` (for plotting)
- `numpy` (for numerical calculations)
- `pandas` (for data reading/processing)
- `glob` & `os` (for file searching, built-in)

## 3. Data Setup
### Required CSV Files
Place all data files in the same folder as your Python script.

#### Mandatory Files:
1. `co2-emissions-emissions-mmtco2.csv` – CO₂ emissions (million metric tons)
2. `population-population-people-in-thousands.csv` – Population (thousands)
3. `gross-domestic-product-gdp-billion-dollars-at-purchasing-power-parities.csv` – GDP (billion USD)
4. Electricity generation files (ending with `generation-bkwh.csv`):
   - `fossil-fuels-generation-bkwh.csv`
   - `nuclear-generation-bkwh.csv`
   - `renewables-generation-bkwh.csv`
   - `hydroelectricity-generation-bkwh.csv`
   - `solar-generation-bkwh.csv`
   - `wind-generation-bkwh.csv`
   - `biomass-and-waste-generation-bkwh.csv`
   - `geothermal-generation-bkwh.csv`
   - `tide-and-wave-generation-bkwh.csv`

## 4. How to Run the Code
### Step 1: Save the Code
Copy all provided code into a single Python file.

### Step 2: Run the Script
Execute the Python script in your development environment.

### Step 3: View Outputs
- Each plot will open in a new window sequentially.
- Close the current plot window to view the next one.
- Plots are automatically saved to your folder.

## 5. Output Description
The script produces 7 visualizations in this order:
1. **Top 20 Countries CO₂ Emissions Bar Chart (2023)**
   Bar chart sorted by total emissions
2. **Full Country CO₂ Bubble Chart (2023)**
   X: Total emissions | Y: Per capita | Size: Population | Color: Emission intensity
3. **16 Countries CO₂ Bubble Chart**
   Excluding China/India/USA/Russia
4. **Saudi Arabia: Total CO₂ vs. Emission Intensity (1980–2023)**
   Saved as `saudi_co2_intensity.png`
5. **Saudi Arabia Electricity Generation (1980–2023)**
   Stacked area: Fossil / Nuclear / Renewables
6. **UK Electricity Generation (1980–2023)**
7. **Saudi Arabia Renewable + Nuclear Breakdown (1980–2023)**
   Detailed stacked area for clean energy

## 6. Notes
*(Original content has no additional notes)*
