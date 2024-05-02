# Image Classification of Erythema
## Distinguishing between Erythema migrans (Lyme Disease rashes) and other rashes using a neural network

It is important to recognize an erythema migrans at an early stage in order to start antibiotic treatment timely and to avoid long-term consequences. Distinguishing the diagnosis from similar-looking skin diseases may be difficult, especially for people without a medical background.

The goal was to build an image classification model that can predict the diagnosis of a skin disease. There are four classes in the model that are trained and can be predicted: erythema migrans, erysipelas, tinea corporis and urticaria. The latter three represent some of the differential diagnoses of erythema migrans.

The target audience of a model like this would be people without any medical background knowledge. The intention of such a model would be to serve as a first screening if the services of the general practioner are not available (e.g. on weekends). If the model would screen positive for an erythema migrans, people could refer to an emergency practice to confirm the diagnosis and, if confirmed, to receive a prescription for antibiotic treatment. The use case of such a model would thus be avoiding the overlooking of erythema rashes or mistaking them for unproblematic rashes in laymen when low-threshold medical services are not readily available.

The dataset was created by means of downloading images from a duckduckgo search. After cleaning of the data, a total set of 623 images resulted (64 images used as the test set, 559 images as the training set).

A neural network for image classification was built in Python using the fastai library. The model was able to classify 81-85% of skin disease images correctly (accuracy of 0.81 on the test set and 0.85 on the validation set). 79% of cases with erythema migrans were detected by the model (sensitivity).

Please note that this model is not intended for medical use in practice.


**Contents of the notebook:**

  - Introduction and relevance of the topic
  - Aim of the model
  - Installation of libraries, imports & credits
  - Dataset
  - Buildung the neural network using transfer learning
  - Evaluation of the model
  - Predictions
  - Limitations
  - Conclusion
  - Bibliography

