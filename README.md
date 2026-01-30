# Hi we are team 12 Sachin Chahal and Margaret DuCasse

Welcome to our Ping Pong game!

Regression Modeling with California Housing Dataset
📊 Dataset

Loaded the California Housing dataset using sklearn.datasets.fetch_california_housing.

Separated the dataset into:

Features (X) — housing attributes

Target (y) — median house value

Printed dataset dimensions to verify successful loading.

🔀 Train–Test Split

Split the dataset into training (80%) and testing (20%) sets.

Used a fixed random_state=42 to ensure reproducibility.

Verified the shapes of all resulting datasets.

🧠 Model: Multi-Layer Perceptron Regressor

Trained a neural network regression model using MLPRegressor.

Configured the model with:

early_stopping=True to prevent overfitting

Custom hidden layer architecture: (10, 5)

max_iter=500

batch_size=1000

activation='relu'

validation_fraction=0.2

Fit the model on the training data.

🔮 Predictions

Generated predictions for:

Training set

Testing set

Used the trained model to compare actual vs. predicted values.

📉 Visualization & Output

Created scatter plots to visualize Actual vs. Predicted values:

One plot for the training set

One plot for the testing set

Included a reference diagonal line (y = x) to indicate perfect predictions.

Saved plots to the figures/ directory:

figures/
├── actual_vs_predicted_train.png
└── actual_vs_predicted_test.png


Ensured figures are high quality using dpi=300.

📁 Project Structure
.
├── src/
│   └── ds_pipeline.py
├── figures/
│   ├── actual_vs_predicted_train.png
│   └── actual_vs_predicted_test.png
├── requirements.txt
└── README.md

⚙️ How to Run
pip install -r requirements.txt
python src/ds_pipeline.py

