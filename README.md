# Pie & AI Kyiv

Materials, code, and Google Colab notebooks from **Pie & AI Kyiv** community events.

## From Data to Prediction

This repository currently contains the materials for **Pie & AI Kyiv: From Data to Prediction**, held online on **16 September 2026** in Ukrainian.

The event demonstrates a complete journey from traditional programming rules to practical machine-learning workflows using real historical market data for Alphabet/Google (`GOOG`).

### Topics covered

- traditional programming rules versus machine learning;
- downloading and exploring financial data with `yfinance`;
- feature engineering with returns, moving averages, volatility, and volume;
- defining a binary next-day `UP`/`DOWN` target;
- understanding weights, bias, sigmoid, loss, gradients, and optimization in PyTorch;
- forecasting a time series with Prophet;
- building and evaluating a neural network with TensorFlow/Keras;
- chronological train, validation, and test splits;
- avoiding data leakage in time-series tasks;
- comparing a model with naive baselines;
- evaluating Accuracy, Precision, Recall, F1 Score, ROC AUC, and a confusion matrix;
- validating results with `TimeSeriesSplit`;
- training logistic regression directly in SQL with BigQuery ML.

## Repository structure

```text
pie-ai-kyiv/
├── README.md
├── LICENSE
└── From-Data-to-Prediction/
    └── Pie_AI_Kyiv_From_Data_to_Prediction.ipynb
```

## Notebook

Open the event notebook:

[Pie AI Kyiv — From Data to Prediction](From-Data-to-Prediction/Pie_AI_Kyiv_From_Data_to_Prediction.ipynb)

The notebook is designed for **Google Colab**. It combines explanatory Markdown cells, visual material, executable Python code, model training, evaluation, and a BigQuery ML demonstration.

## Technologies

- Python
- pandas
- NumPy
- Matplotlib
- yfinance
- PyTorch
- Prophet
- TensorFlow / Keras
- scikit-learn
- Google Colab
- Google Cloud BigQuery
- BigQuery ML
- SQL

## Running the notebook

1. Open the `.ipynb` file in GitHub.
2. Select **Open in Colab**, or upload the notebook manually to [Google Colab](https://colab.research.google.com/).
3. Run the cells from top to bottom.
4. When prompted, allow installation of the required packages.
5. The BigQuery ML section requires access to a Google Cloud project with BigQuery enabled.

The main additional packages can be installed with:

```python
!pip -q install yfinance prophet
```

## Learning objective

The purpose of this project is not to produce a trading system. It is to demonstrate how a real dataset becomes a machine-learning problem and how model results should be validated and interpreted critically.

The central takeaway is simple:

> A more complex model does not automatically produce a better forecast.

Correct problem formulation, feature quality, chronological validation, prevention of data leakage, and comparison with simple baselines are often more important than model complexity.

## Important notes

- Market data may change when the notebook is rerun because `yfinance` downloads the latest available observations.
- Random initialization may cause small differences in neural-network results across environments.
- Prophet produces a time-series trajectory, while the TensorFlow/Keras and BigQuery ML examples address next-day directional classification.
- BigQuery resources and project identifiers may need to be replaced with your own Google Cloud configuration.

## Educational disclaimer

This repository is provided for educational and demonstration purposes only. The code, models, forecasts, metrics, and examples are **not investment advice, financial advice, or a ready-to-use trading strategy**.

## Author and event host

**Valentyn Verovkin**  
Pie & AI Kyiv event organizer and presenter

## Language

The event presentation and explanatory materials are primarily in **Ukrainian**. Code, variable names, and technical terminology may also appear in English.

## License

The project is distributed under the [MIT License](LICENSE).

## Feedback

Questions, suggestions, and ideas for future Pie & AI Kyiv events are welcome through GitHub Issues.
