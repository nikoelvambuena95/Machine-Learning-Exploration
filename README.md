# Machine Learning - Exploration
This repo is an ongoing exploration of Machine Learning models.
<br>
<br>
Current objectives:
- Unsupervised models
- Hyperparameter Tuning

### Multi-Linear Regression
Not the best model because of its low r-score: 0.104...

The multi_linear regression is better suited for "binary problems".

The dataset we have is more aligned with a classification model.

### KNN
The KNN model produce a moderate, initial r-score: 0.832...

Parameters were adjusted by importing GridSearchCV.
These parameters were:
- n_neighbors
- weights
- algorithm

After parameter adjustment, there was a small increase in r-score: 0.837...
```python 
best given parameters: {'algorithm': 'auto', 'n_neighbors': 11, 'weights': 'distance'} 
```

### Keras
Accuracy below 0.84 prior to adjusting 'number_hidden_nodes' parameter.

Adjusted 'number_hidden_nodes' from 4 to 100, accuracy increased to 0.88 with a loss of 1.11.
```python

from tensorflow.keras.layers import Dense
number_inputs = 40
number_hidden_nodes = 100
keras.add(Dense(units=number_hidden_nodes,
                activation='relu', input_dim=number_inputs))
```

### Conclusion
The <b>keras</b> model seems to be the <b>best performing</b> model in terms of accuracy.

---
### Contact
LinkedIn | https://www.linkedin.com/in/niko-elvambuena/
<br>
Email | niko.elvambuena95@gmail.com
