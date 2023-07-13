# Fingertips Position Estimation of a Robot Hand

## Project Description: In this project, the goal is to achieve the lowest RMSE for the task of Fingertips Position Estimation of a robot hand using the dataset provided.

## Project Evaluation: The evaluation metric used will be root mean squared error, i.e., a measure of the root of the average squared difference between the observed and predicted values. You should use the format specified in the submission evaluation code for making a submission. The first column consists of the sample ID, while the remaining 12 hold the fingertip position values.


In my project, I utilized a Kaggle notebook for efficient coding. The approach combined CNN and RNN methodologies to address the problem at hand effectively.

The CNN component began with three convolutional layers. The first layer applied a kernel size of 5 and padding of 2 to extract features from the data. The subsequent layer employed a kernel size of 5 and padding of 1 to further refine these features. Finally, a convolution operation with a kernel size of 2 and padding of 1 was applied to capture fine-grained details. The purpose of these convolutional layers was to identify important patterns and structures in the data.

Following the CNN layers, a fully connected layer was introduced to expand the extracted features and capture complex relationships between them. This layer enhanced the model's ability to learn higher-level abstractions from the data.

To incorporate temporal information, an LSTM layer was used. LSTMs exceled at capturing long-term dependencies and timing information in sequential data. By utilizing an LSTM layer, the model can effectively learn and understand temporal patterns within the data.

The project involved performing regression prediction for 12 consecutive points. To train the model, the Mean Squared Error (MSE) loss function was employed. MSE was commonly used for regression tasks as it quantified the average squared difference between predicted and actual values, providing a measure of the model's performance.

To optimize the model's parameters, stochastic gradient descent (SGD) was employed due to the large dataset. SGD randomly selected subsets of the data for each iteration, making it computationally efficient for training on large datasets.
