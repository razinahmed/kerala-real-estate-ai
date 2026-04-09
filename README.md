# Kerala Real Estate AI

> AI-powered property price prediction for the Kerala housing market using machine learning.

![Python](https://img.shields.io/badge/Python-3.9+-blue)
![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-orange)
![License](https://img.shields.io/badge/License-MIT-green)

## Overview

Kerala Real Estate AI predicts property prices across Kerala districts using a Linear Regression model trained on historical housing data. Input features include district location, square footage, and number of bedrooms. The model is trained on real market data from major Kerala cities including Kochi, Trivandrum, and Kozhikode.

## Features

- Property price prediction using Linear Regression
- District-wise price modeling for Kerala housing market
- CSV-based dataset with real market indicators
- Support for multiple input features: district, area (sqft), bedrooms
- Lightweight and fast inference with scikit-learn

## Tech Stack

- **Language**: Python 3.9+
- **ML Library**: scikit-learn (Linear Regression)
- **Data Processing**: pandas
- **Data Format**: CSV
- **Build**: Makefile

## Quick Start

```bash
# Clone the repository
git clone https://github.com/razinahmed/kerala-real-estate-ai.git
cd kerala-real-estate-ai

# Install dependencies
pip install pandas scikit-learn

# Run the predictor
python predictor.py
```

## Dataset

The training data is located in `data/prices.csv` with the following schema:

| Column | Type | Description |
|--------|------|-------------|
| `district` | string | Kerala district name (Kochi, Trivandrum, Kozhikode) |
| `sqft` | integer | Property area in square feet |
| `bedrooms` | integer | Number of bedrooms |
| `price` | integer | Property price in INR |

## Project Structure

```
kerala-real-estate-ai/
├── predictor.py        # ML model training and prediction
├── data/
│   └── prices.csv      # Kerala property price dataset
├── Makefile            # Build and test commands
├── LICENSE             # MIT License
├── SECURITY.md         # Security policy
└── README.md           # Project documentation
```

## Extending the Dataset

Add new rows to `data/prices.csv` to improve model accuracy:

```csv
Alappuzha,1400,2,4800000
Thrissur,1600,3,6200000
```

## Contributing

Contributions are welcome. Fork the repository, create a feature branch, and submit a pull request.

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
