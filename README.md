# Neural Network Charity Analysis

## Overview of the analysis
The company, Alphabet Soup, send a CSV data set with over 34,000 organizations that have been given funding from the company. We used machine learning and neural networks to create a binary classifier to predict if applicants are successful if Alphabet Soup provides funding.

In this analysis we:
- Preprocessed the data for a neural network model
- Compiled, trained, and evaluated the model
- Optimized the model

## Results

### Data Preprocessing
- The "IS SUCESSFUL" column is the target for our model.
- We used "APPLICATION TYPE", "AFFLILIATION", "CLASSIFICATION", "USE CASE", "ORGANIZATION", "INCOME AMOUNT", AND "SPECIAL CONSIDERATIONS" as our features for the model.
- We dropped the "EIN" and "NAME" colums from our dataset as they were not necessary for our model.
![featured](https://github.com/amiecostello22/Neural_Network_Charity_Analysis/blob/main/images/featured.png)
![drop](https://github.com/amiecostello22/Neural_Network_Charity_Analysis/blob/main/images/drop.png)

### Compiling, Training, and Evaluating the Model
- We used two hidden layers and an output layer. The first hidden layer had 80 neurons and used a ReLU function. The second layer had 30 neurons and also used a ReLU function so all neurons would not activate all at once. We used the Sigmoid funtion on the output layer as our activation function.
- The model had an accuracy level of 73 and did not achieve the target model performance.
- In attempt to increase the model performance, we used four layers each starting with a larger neuron count than the first model. The first two layers used the ReLU function, then we used the Sigmoid function on the final two layers, and used the Linear function on the Output layer.

![layers](https://github.com/amiecostello22/Neural_Network_Charity_Analysis/blob/main/images/layers.png)
![increased_layers](https://github.com/amiecostello22/Neural_Network_Charity_Analysis/blob/main/images/increased_layers.png)


## Summary
Using the ReLU and Sigmoid functions our model had an accuracy of only 73 despite increasing the number of neurons and layers. We could try to rework the data using a SVM, Support Vector Machine. Neural Networks and Deep Learning Models can focus on a specific trend and miss the overall trend we are seeking. SVMs are also not as prone to overfitting the data as Neural Networks and Deap Learning Models. It takes all the data within a boundary to create a larger seperation between the classifications. 

