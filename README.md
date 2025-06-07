# Ethanol-ANN-model 
# Bioethanol Concentration Prediction Using ANN

This repository contains the work done as part of an academic OJT and project under the guidance of Dr. Tejaswini Pachpor at MIT-WPU, Pune. The project involves building an artificial neural network (ANN) model to predict and optimize the concentration of bioethanol produced during industrial-scale fermentation, using real operational data obtained from a sugar mill.

The bioethanol industry in India is growing rapidly due to its role in renewable energy and reducing dependency on fossil fuels. Optimizing ethanol yield through predictive modeling can contribute significantly to improving production efficiency. This project attempts to integrate domain knowledge with data-driven approaches to derive meaningful insights and operational improvements.

# Project Title

Model construction and optimization for raising the concentration of industrial bioethanol production by using a data-driven ANN model

# Objective

- To study the effect of different process variables on the bioethanol concentration.
- To apply ANN modeling using real-time industrial data to predict bioethanol yield.
- To identify optimum input conditions for maximizing bioethanol concentration.

# Data Description

The dataset includes 13 process-related variables collected from a working sugar mill's bioethanol production unit. These variables capture fermentation parameters, sugar content in raw and processed materials, and physicochemical conditions.

##Feature Selection

Using Pearson correlation matrix and domain understanding, the following six variables were selected for model input. These features showed either a strong or moderate correlation with the target (BEC) and were relatively independent of one another, reducing redundancy and multicollinearity in the model.

Selected input features:

- `YV` – Concentration of cells in yeast vessels (correlation with BEC: 0.30)
- `FM` – Concentration of cells in fermenters (correlation with BEC: 0.55)
- `TSSFMWD` – Total suspended solids of fermented wash before decanter (correlation with BEC: 0.32)
- `TSCWAD` – TSS of clarified wash after decanter (correlation with BEC: 0.39)
- `TRSMRP` – TRS (total reducing sugars) of molasses received for processing (correlation with BEC: 0.56)
- `WFMpH` – pH of fermentation water (correlation with BEC: -0.56, showing a strong negative correlation)

Output variable:

- `BEC` – Bioethanol concentration (target variable for prediction)

# Work Done So Far

- Completed data visualization using Seaborn pairplot
- Performed Pearson correlation analysis
- Selected six independent input variables based on correlation with BEC
- Normalized the selected features using MinMaxScaler
- Saved normalized dataset for model input

# Tools Used

- Python (Pandas, Seaborn, Matplotlib)
- Scikit-learn (for normalization)
- Google Colab
- ChatGPT
- TensorFlow / Keras (upcoming)


# Upcoming Tasks

- Building and training the ANN model using Keras
- Evaluating model performance using R² and MSE
- Visualizing predicted vs actual BEC values
- Hyperparameter tuning




