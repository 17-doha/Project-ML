Name
=======
**Mobile Health Analysis**

Description
=======
A Project that combines data cleaning, data visualization, and feature engineering to present the best machine learning model by comparing different models for deciding the specific activity according to the sensors’  data.

**Dataset Exploration:**
* Explored the dataset by visualizing the Activity column which is my target and found the problem of biased sampling as class 0 has the most features and this could lead to problems in accuracy.
* Prepared a balanced data through downsampling technique by taking equal sample of each class with the count of the minority class in the Activity column.
* Figured out the outliers in the data and removed the outlier to prevent any error could occur while normalizing the data.
* Dropped subject column.
* Performing PCA on the features of the data and selecting 3 principal components from them and then visualizing them in 3D.
![image](https://github.com/17-doha/Project-ML/assets/65771031/c47869d5-dc2b-420d-8bff-bc2d6609c38c)

* Performing StandardScaler normalization on the data.
* Model Training and Model Evaluation:
* KNN model with accuracy 94.3% at k = 7.
![image](https://github.com/17-doha/Project-ML/assets/65771031/8911b549-ea73-4acb-9c15-f0b3190724d2)
* SVM model with RBF kernel with accuracy 92.3%
![image](https://github.com/17-doha/Project-ML/assets/65771031/20f54b33-638f-419a-9fe7-350625ff17e8)
* Linear Regression Model → MSE of 8.71
* Ridge Regression Model with an alpha of 0.01 →  MSE of 8.71
* Lasso Regression Model with an alpha or 0.0001 → MSE of 8.71
* Logistic Regression Model → Accuracy of 60%
![image](https://github.com/17-doha/Project-ML/assets/65771031/74836c2c-f204-4231-a270-46fd18f32a2d)
* Neural Networks Model with 3 layers first layer of 64 neuron and relu activation function, second layer of 64 neuron and relu activation function, and the last layer of 13 neuron and softmax activation function. Optimizer ADAM, loss function categorical-crossentropy, and 30 epochs. → Accuracy of 94.3%
![image](https://github.com/17-doha/Project-ML/assets/65771031/9f0f9ed9-5b4c-4185-91f3-228609498a73)
**Result Analysis:**
* In conclusion KNN, SVM, Neural Networks are the best for this dataset considering time and accuracy.
* The best Model with this dataset is is Neural Networks achieving the highest accuracy and nearly average time.

