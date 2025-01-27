## Quantifying_Uncertainty_in_Neural_Networks

Neural network model predictions can be underconfident (when the predicted confidence of the model is less than the true likelihood of the
event) or overconfident, that means the model is badly calibrated. This marks the importance of having the uncertainty estimate for the
neural networks.

Uncertainties can be of different types:
1. Aleatoric uncertainty (Data-Dependent Uncertainty): It arises from inherent randomness or variability in the data itself, such as
measurement noise or inherent variability in the data distribution. This is irreducible uncertainty as it arises from the natural complexity of
the data, such as class overlap, label noise, homoscedastic and heteroscedastic noise.

2. Epistemic uncertainty (Model-Dependent Uncertainty) : It measures the uncertainty in estimating the model parameters given the
training data - this measures how well the model is matched to the data. Thus, it reflects the model’s inability to perfectly capture the
underlying relationship between the input features and the target variable. Model uncertainty is reducible as the size of training data
increases.

Following is the process we followed to quantify Data Uncertainty and Model Uncertainty in the Neural Network where we have a base neural network architecture and on top of which we append another layer that helps us to quantify uncertainty:

<img width="669" alt="flow" src="https://github.com/user-attachments/assets/590a7508-4d19-4bb2-a66c-85219b9e2e33" />

