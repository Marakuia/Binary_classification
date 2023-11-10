# Binary_classification

In this work, three models of fully connected neural networks were implemented to solve the binary classification problem. <br/>
The training was carried out on a dataset based on data on the reflection of radar signals from the surfaces of stones and metal cylinders. 60 input values indicate the strength of the reflected signal at a certain angle. The input data is normalized and ranges from 0 to 1. <br/>

The models were implemented using the Keras library. The work uses the Adam optimizer, binary cross-entropy is used as a loss function, and accuracy is used as a metric. <br/>

The first model receives all the features, including redundant ones, that describe the same signal from different angles. <br/>
Graphs of the loss function and accuracy versus epoch for the first model are presented below. <br/>
<img src="https://github.com/Marakuia/Binary_classification/blob/main/result/model1.png" width="500" height="800">

When implementing the second model, redundancy was taken into account and eliminated by reducing the number of significant features in the input layer. The error and accuracy of the second model are slightly worse than the first, but this may be due to the lack of overfitting, which the first model is prone to. <br/>
Graphs of the loss function and accuracy versus epoch for the second model are presented below. <br/>
<img src="https://github.com/Marakuia/Binary_classification/blob/main/result/model2.png" width="500" height="800">

In the third model, a hidden layer was added, which made it possible to find patterns not only in the input data, but also in their combinations.
Graphs of the loss function and accuracy versus epoch for the third model are presented below. <br/>
<img src="https://github.com/Marakuia/Binary_classification/blob/main/result/model3.png" width="500" height="800">

With the redundancy removed and the hidden layer added, the latter model performed the best.
