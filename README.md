# 🌦️ City Temperature Monitoring System

**A C-based console application for analyzing, visualizing, and forecasting weather data.**

## 📖 Overview
The **City Temperature Monitoring System** is a comprehensive tool designed to simulate and analyze meteorological data. It processes daily temperature readings across 12 months and weekly rainfall data for a year. The system provides statistical insights, visual graphs using ASCII art, weather forecasting, and interactive educational games.

## 🚀 Key Features

### 📊 Data Analysis
* **Overview:** Calculates Year-Max, Year-Min, and Year-Average temperatures.
* **Monthly Statistics:** Detailed breakdown (Min/Max/Avg) for specific months.
* **Trend Analysis:** Compares current month averages with previous/next months to determine warming or cooling trends.
* **Deviations:** Calculates temperature deviation from the mean for specific days or months.
* **Streak Detection:** Identifies the longest consecutive run of Hot (>35°C) or Cold (<10°C) days.
* **Seasonal Analysis:** Breaks down data based on IMD standards (Winter, Summer, Monsoon, Post-Monsoon).

### ⚠️ Alerts & Safety
* **Heatwave/Coldwave Detection:** Analyzes 3-day rolling averages to issue warnings.
* **Flood Alerts:** Monitors weekly rainfall data (>900mm) to predict potential flooding.

### 🔮 Forecasting
* **Linear Regression:** Uses statistical logic to predict future temperatures based on existing daily data trends.

### 🌧️ Rainfall Module
* **Weekly Data:** Visualizes rainfall intensity using ASCII icons (`🌧️`).
* **Humidity Reports:** Classifies months as Dry, Moderate, or Humid based on temperature and rainfall correlation.

### 🎮 Gamification
* **Trivia Quiz:** Tests meteorological knowledge.
* **Guess the Temp:** Players guess the average temperature of a specific month.
* **Memory Game:** Tests the user's ability to recall numerical weather sequences.

## 🛠️ Technical Details
* **Language:** C
* **Interface:** CLI (Command Line Interface) with ANSI Color codes.
* **Data Structure:**
    * 2D Arrays (`temp[12][30]`) for daily temperature.
    * 1D Arrays (`rf[52]`) for weekly rainfall.
* **Platform:** Optimized for **Linux/Unix** (uses `unistd.h` and `system("clear")`).

## 🔐 Credentials
The system is protected by a login screen. Use the default credentials to access the dashboard:

| Field | Default Value |
| :--- | :--- |
| **Username** | `admin` |
| **Password** | `1234` |

## ⚙️ Installation & Usage

### Prerequisites
* GCC Compiler (or any standard C compiler).
* A terminal that supports ANSI escape codes (Git Bash, VS Code Terminal, or Linux Terminal).

### Compilation
1.  Open your terminal in the project folder.
2.  Compile the code:
    ```bash
    gcc finalll.c -o weather_system
    ```

### Execution
Run the executable:
```bash
./weather_system