# Power-Plant-Energy-Output-Prediction-ANN

📌 Power Plant Energy Output Prediction (ANN)

📖 Overview
This project predicts the electrical energy output (PE) of a power plant using an Artificial Neural Network (ANN).
The model is trained on environmental factors like temperature, exhaust vacuum, ambient pressure, and humidity.

📊 Dataset
File: powerplant_data.csv
Features:
  AT → Ambient Temperature
  V → Exhaust Vacuum
  AP → Ambient Pressure
  RH → Relative Humidity
Target:
  PE → Power Output

⚙️ Tech Stack
  Python
  Pandas
  Scikit-learn
  PyTorch
  
🧠 Model Architecture
  Input Layer (4 features)
          ↓
  Hidden Layer 1 (6 neurons, ReLU)
          ↓
  Hidden Layer 2 (6 neurons, ReLU)
          ↓
  Output Layer (1 neuron)
  
🔄 Workflow
  - Data Loading & Exploration
  - Train-Test Split (80-20)
  - Feature Scaling using StandardScaler
  - Conversion to PyTorch Tensors
  Model Training using:
    Loss: MSELoss
    Optimizer: Adam
  Model Saving (best validation loss)
  Evaluation using MSE & R² Score

📉 Training Performance
  Final Train MSE: 21.21
  Final Test MSE: 19.37
  R² Score: 0.93

👉 The model explains ~93% variance in power output, which indicates strong performance.

📌 Key Learnings
  Importance of feature scaling in neural networks
  Difference between training & validation loss
  Model checkpointing (saving best model)
  Regression evaluation using MSE & R²

🤝 Contributing
  Pull requests are welcome!
