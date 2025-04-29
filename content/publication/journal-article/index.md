---
title: "Electric Load Forecasting Enhanced by Weather Factors: A Comparative Study of GRU, LSTM, and XGBoost Model in Jamali Power System Network"
authors:
- admin
author_notes:
- "Equal contribution"
- "Equal contribution"
date: "2025-09-01T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: ''

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["article-journal"]

# Publication name and optional abbreviated publication name.
publication: "*The 3rd International Conference on High Voltage Engineering and Power Systems"
publication_short: ""

abstract: Electric load forecasting plays a critical role in efficient energy management, helping utility companies balance supply and demand, reduce operational costs, and maintain grid stability. This paper provides a comparative analysis of three predictive models—GRU, LSTM, and XGBoost—to identify the most accurate model for electric load forecasting using time-series data, including historical load data and weather factors such as temperature, humidity, and wind speed. The models were evaluated on metrics including R², MAPE, RMSE, and MAE. Results show that GRU outperforms both LSTM and XGBoost, achieving the highest R² value of 0.990 and a MAPE of 0.79 %, indicating its superior ability to capture complex temporal dependencies in the load data. The LSTM model closely follows with an R² of 0.989 and MAPE of 0.85 %, while XGBoost lags with an R² of 0.589 and a MAPE of 4.76 %, demonstrating its limitations in time-series forecasting. Hyperparameter tuning played a crucial role in optimizing model performance, with GRU's simpler architecture providing a slight edge over LSTM. These findings establish the GRU model as the most reliable and accurate model for electric load forecasting for this case, particularly when accounting for both historical load patterns and weather-related variables, highlighting the importance of recurrent neural networks for this application.

# Summary. An optional shortened abstract.
summary: This study compares GRU, LSTM, and XGBoost for electric load forecasting, concluding GRU achieves the highest accuracy by effectively capturing historical load patterns and weather influences.

tags:
- Source Themes
featured: false

# links:
# - name: ""
#   url: ""
url_pdf: ''
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photosphoto-of-truss-towers-yETqkLnhsUI)'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: example
---


