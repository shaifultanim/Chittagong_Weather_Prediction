
 🌦️ Chittagong Weather Predictor
 
 ![Python](https://img.shields.io/badge/python-3.10%2B-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Data](https://img.shields.io/badge/dataset-2010--2022-orange)
![Status](https://img.shields.io/badge/status-active-brightgreen)

_A Python-based tool for analyzing and predicting weather patterns in Chattogram, Bangladesh using historical data (2010-2022)

![image](https://github.com/user-attachments/assets/f7fb36a9-bf79-4038-947a-4e7915c27e4a)

 📖 Table of Contents
- [Features](-features)
- [Installation](-installation)
- [Usage](-usage)
- [Data Requirements](-data-requirements)
- [How It Works](-how-it-works)
- [Contributing](-contributing)
- [License](-license)

 ✨ Features
- Historical Weather Lookup: Retrieve exact weather data for dates between 2010-2022
- Future Predictions: Estimate weather using same-date historical averages
- Visual Forecasts: 24-hour temperature fluctuation graphs
- Practical Advice: Weather-specific recommendations (umbrella alerts, etc.)
- Error-Resilient: Handles missing data and invalid inputs gracefully

 💻 Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/chattogram-weather.git
   cd chattogram-weather
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Place your weather data CSV in the `data/` folder

 🚀 Usage
Run the predictor:
```bash
python weather_predictor.py
```

Example Session:
```
==================================================
Chattogram Weather Forecast (2010-2022)
==================================================

Enter a date (MM-DD-YYYY) or 'q' to quit: 06-15-2020

Observed Weather on 06-15-2020:
Condition: Rain
Temperature: 28.5°C (Range: 26.7°C to 30.2°C)
Humidity: 85%

Advice: Carry an umbrella and wear waterproof shoes!
```
(Graph window will open automatically)

 📂 Data Requirements
Place this file in `data/` folder:
```
Chittagong Weather Data 2010-01-01 to 2022-08-22.csv
```

Required Columns:
| Column      | Format          | Example       |
|-------------|-----------------|---------------|
| `datetime`  | MM/DD/YYYY      | 06/15/2020    |
| `temp`      | Temperature (°C)| 28.5          |
| `humidity`  | Percentage      | 85            |
| `conditions`| Text description| "Rain"        |

 🔧 How It Works
1. Data Loading: Reads historical CSV data
2. Date Processing:
   - Exact matches show recorded data
   - Future dates use same-day historical averages
3. Prediction Engine:
   - Generates realistic hourly temperature fluctuations
   - Provides condition-based advice
4. Visualization: Matplotlib graphs with enhanced styling

 🤝 Contributing
1. Fork the repository
2. Create your feature branch:
   ```bash
   git checkout -b feature/new-feature
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add new feature"
   ```
4. Push to the branch:
   ```bash
   git push origin feature/new-feature
   ```
5. Open a pull request

 📜 License
MIT License - See [LICENSE](https://github.com/Souad-Hasan/Chittagong-Climate-Predictor/blob/ee18594b69c0aa9f26bd5c9cda9c018c0b015950/MIT%20license.txt) for details

---

Dataset Source: [Kaggle - Chittagong Weather Data](https://www.kaggle.com/datasets/mohammadsadmantahsin/chittagong-weather-data-from-2000-to-2020)
