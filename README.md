# Advanced Contextual Farming System (Crop Recommender System)

This project is an advanced contextual farming system that helps farmers and agricultural stakeholders make data-driven decisions. It provides Machine Learning-based recommendations for crop selection and crop yield prediction. Additionally, it features weather forecasting capabilities.

## Features

- **Crop Recommendation**: Predicts the most suitable crop to grow based on specific features like soil nutrients and environmental factors.
- **Crop Yield Prediction**: Estimates the crop yield using parameters such as State, Crop Type, Area, and Soil Type.
- **Weather Forecasting**: Provides current and upcoming weather data for a specific location using the OpenWeather API.
- **Interactive Web Dashboard**: A Flask-based web application with an easy-to-use interface for uploading data, visualizing charts, and making predictions.
- **CSV Data Preview**: Upload and preview datasets directly in the dashboard.

## Tech Stack

- **Backend Framework**: Flask (Python 3.8)
- **Machine Learning**: Scikit-Learn, Pandas, NumPy
- **Models**: Pre-trained Random Forest/Decision Tree models (Pickle format - `crop.pkl`, `yield.pkl`)
- **Frontend**: HTML templates, CSS (Static files), Jinja2
- **External API**: OpenWeather API (for weather forecasts)

## Prerequisites

- [Python 3.8](https://www.python.org/downloads/release/python-380/)
- Pip (Python Package Installer)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/hiba06/advanced-contextual-farming-system.git
   cd advanced-contextual-farming-system
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
   *(Note: The requirements include `pandas`, `numpy`, `scikit-learn==0.23.1`, `flask`, and `matplotlib`.)*

3. Configure Weather API:
   - Ensure the `config/config.cfg` file contains valid API credentials (API_KEY and API_URL) for the OpenWeather API.

4. Run the application:
   ```bash
   python app.py
   ```

5. Open your web browser and navigate to:
   ```
   http://127.0.0.1:5000/
   ```

## Usage

- **Home/Index**: Introduction to the platform.
- **Crop Prediction**: Navigate to the crop prediction module, input environmental and soil data to get the recommended crop.
- **Yield Prediction**: Enter details such as state, crop, area, and soil type to get the estimated yield.
- **Weather**: Check current and upcoming weather data by entering your location.
- **Upload & Preview**: Upload a `.csv` file to preview its contents directly inside the application.

## Models Overview

- `crop.pkl`: Pickled machine learning model utilized for recommending the best crop based on given parameters.
- `yield.pkl`: Pickled machine learning model trained to estimate the crop yield in a given area for a selected crop.

## License

This project is open-source and available under the standard MIT License.
