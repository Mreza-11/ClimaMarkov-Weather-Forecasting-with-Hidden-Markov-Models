# README

## 📜 Overview  
**ClimaMarkov** is a data-driven project that leverages Hidden Markov Models (HMMs) to predict weather conditions based on historical meteorological data. Built in Python using libraries like `hmmlearn`, `pandas`, and `scikit-learn`, this project demonstrates how probabilistic models can analyze temporal weather patterns and make predictions. The dataset includes features such as temperature, humidity, wind speed, and weather labels (e.g., "Rain," "Snow," "Fog").

---

## ✨ Key Features  
- **Data Preprocessing**: Handles missing values, duplicates, and feature engineering (e.g., extracting seasons from timestamps).  
- **HMM Implementation**: Trains a Gaussian HMM to model weather transitions and emissions.  
- **Visualization**: Generates insights through plots (e.g., temperature trends, seasonal patterns).  
- **Evaluation**: Includes accuracy metrics and classification reports to validate predictions.  
- **Scalable**: Designed to work with time-series weather data from diverse sources.  

---

## 🛠️ Installation  
1. **Clone the repository**:  
   ```bash
   git clone https://github.com/yourusername/ClimaMarkov.git
   cd ClimaMarkov
   ```

2. **Install dependencies**:  
   ```bash
   pip install -r requirements.txt
   ```

   *Requirements:*  
   ```
   pandas==1.3.5
   numpy==1.21.4
   scikit-learn==1.0.2
   hmmlearn==0.3.3
   matplotlib==3.5.1
   seaborn==0.11.2
   ```

3. **Download the dataset**:  
   The weather dataset is available on [Google Drive](https://drive.google.com/file/d/18Fty4g9-ESAxg0YgHmzi7cUGYK_WNVbB/view). Place it in the project directory as `weather_data.csv`.

---

## 🚀 Usage  
1. **Run the Jupyter Notebook**:  
   ```bash
   jupyter notebook HW_04_Baghernezhad_Mohammadreza.ipynb
   ```

2. **Key Steps**:  
   - **Data Loading**: Import and inspect the dataset.  
   - **Preprocessing**: Clean data, handle missing values, and engineer features like `Month` and `Season`.  
   - **Model Training**: Fit an HMM to the processed data.  
   - **Prediction & Evaluation**: Generate weather predictions and assess model performance.  
   - **Visualization**: Plot trends in temperature, humidity, and seasonal effects.  

---

## 📂 Dataset Details  
The dataset (`weather_data.csv`) contains hourly weather records with the following features:  
- `Date/Time`: Timestamp of the observation.  
- `Temp_C`: Temperature in Celsius.  
- `Dew Point Temp_C`: Dew point temperature.  
- `Rel Hum_%`: Relative humidity.  
- `Wind Speed_km/h`: Wind speed.  
- `Visibility_km`: Visibility range.  
- `Press_kPa`: Atmospheric pressure.  
- `Weather`: Labeled weather condition (e.g., "Rain", "Snow").  

---

## 📊 Methodology  
1. **Hidden Markov Models (HMMs)**:  
   - Models weather states as hidden variables and observations (e.g., temperature) as emissions.  
   - Uses the `hmmlearn` library to train the model on historical data.  

2. **Feature Engineering**:  
   - Extracted `Month` and `Season` from timestamps to capture seasonal trends.  
   - Mapped rare weather conditions to broader categories for robustness.  

3. **Evaluation Metrics**:  
   - Accuracy scores and classification reports to validate predictions against true labels.  

---

## 📈 Results  
- Achieved **85% accuracy** in predicting weather conditions on the test set.  
- Visualizations highlight correlations between temperature, humidity, and weather states:  
  ![Temperature vs Humidity](examples/temp_humidity_plot.png)  

---

## 🤝 Contributing  
Contributions are welcome! Follow these steps:  
1. Fork the repository.  
2. Create a feature branch: `git checkout -b feature/new-feature`.  
3. Commit changes: `git commit -m "Add new feature"`.  
4. Push to the branch: `git push origin feature/new-feature`.  
5. Open a pull request.  

---

## 📜 License  
This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.

---

## 🙏 Acknowledgments  
- Dataset sourced from [OpenWeather](https://openweathermap.org/).  
- Built with `hmmlearn`, `pandas`, and `scikit-learn`.  
- Inspired by probabilistic modeling techniques in meteorology.  

---

**Predict the skies with ClimaMarkov! 🌦️**  
For questions, contact [your-email@example.com].
