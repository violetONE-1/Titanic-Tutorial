# Titanic-Tutorial

Motivation and Overview:

To better gap the bridge between theory and practice of Pytorch learning, I designed this project independently to predict passenger survival based on features like age, sex and title.


Feature Engineering & Preprocessing:

To improve model performance from the baseline, I implemented several key data transformations:

Title Extraction: Extracted social titles (Mr, Miss, etc.) from passenger names and mapped them to numerical categories.

Missing Value Imputation: Used median values to fill gaps in 'Age' and 'Fare' to maintain data integrity.

Feature Scaling: Normalized continuous variables (Age, Fare) to ensure stable gradient descent during training.


Challenges and Solutions:

During the development, I encountered and resolved several technical challenges that demonstrate a deep understanding of the deep learning pipeline:Overfitting on Small Dataset. Noticed a drop in Kaggle leaderboard accuracy after adding complex features. Addressed this by simplifying the network architecture to 3 layers, adding Dropout (p=0.2) to improve generalization and appropriately reducing the number of training epochs.

Result:

Best Accuracy: ~80% on the public leaderboard.
And I realized that in small-scale datasets like Titanic, robust feature engineering and regularization are often more effective than increasing model depth.

<img width="1798" height="484" alt="0bdcd94f-5e26-479b-9d30-0cb237091e67" src="https://github.com/user-attachments/assets/22f173e3-4164-4784-acbb-48832ee5beb4" />

