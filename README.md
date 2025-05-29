### HOME ASSIGNMENT1

 # Overview
This project includes 3 TensorFlow tasks:
1. Tensor Manipulations & Reshaping
2. Loss Functions Comparison
3. Training a Neural Network with TensorBoard

 # Contents and explaination
  # `tensor_manipulation.ipynb` – Tensor reshaping and broadcasting.
  we demonstrate some fundamental tensor operations using TensorFlow.
First, we create a random tensor with shape 4 by 6, then check its rank, which is the number of dimensions, and its shape.
Next, we reshape this tensor into a 3-dimensional tensor with shape 2 by 3 by 4. Reshaping lets us reorganize the data without changing its content.
Then, we transpose the reshaped tensor, swapping the first two dimensions to get a new shape of 3 by 2 by 4. Transposing rearranges axes, which is useful for aligning data in various ways.
After that, we take a smaller tensor of shape 1 by 4 and broadcast it to match the larger tensor's shape.
Broadcasting automatically expands the smaller tensor across dimensions without copying data.
Finally, we add the broadcasted tensor to the transposed tensor, showing how element-wise operations work seamlessly with broadcasting.
These operations are essential building blocks for manipulating data in deep learning workflows."
  # `loss_functions.ipynb` – MSE vs Cross Entropy loss comparison.
  we compare two common loss functions-Mean Squared Error (MSE) and Categorical Cross-Entropy (CCE)—to understand how they evaluate model predictions.
We start with true labels that are one-hot encoded, representing the correct class. Then we have two model predictions: one that is close to the true label and one that is less accurate.
We calculate both MSE and CCE losses for these predictions. The key idea is that a better prediction should have a lower loss value. As expected, the first prediction has lower MSE and CCE values compared to the second, indicating it's closer to the true label.
Finally, we visualize these loss values side-by-side in a bar chart, showing how both loss functions assign higher penalties to worse predictions.
This helps us understand which loss function might be more sensitive or suitable depending on the
problem."
  # 'mnist_tensorboard.ipynb` – MNIST model training with TensorBoard logging.
  We train a simple neural network to recognize handwritten digits using TensorFlow and visualize the process with TensorBoard.
First, we load the MNIST dataset, which contains thousands of 28x28 pixel images of digits 0-9, and normalize the pixel values to between 0 and 1 for better training.
Next, we build a neural network with an input layer, a hidden dense layer of 128 neurons with ReLU activation, dropout for regularization, and an output layer with softmax to classify digits.
We compile the model using the Adam optimizer and categorical cross-entropy loss, then set up TensorBoard logging to track training metrics like accuracy and loss.
We train the model for a few epochs, validating it on test data. Finally, we launch TensorBoard, which shows interactive graphs of the training progress, helping us understand how well the model learns over time.
  

 # Student Info
- **Name: Vaishnavi Gopi** 
- **Student ID: 700754518**  
- **Course: Neural Networksand Deep Learning**
   
  

## 📽️ Demo Video
Link: https://drive.google.com/file/d/14GRjUnWNjrQZkpyUd2_heOwJ__CvPS1Q/view?usp=drivesdk

## 📝 How to Run
1. Open the notebooks in Google Colab.
2. Run each cell in order.
3. For the last notebook, `%tensorboard --logdir` will launch TensorBoard.

---

### Assignment Questions & Answers

# 1. What patterns do you observe in the training and validation accuracy curves?
In TensorBoard, training accuracy increases steadily, while validation accuracy rises more slowly. If validation starts to plateau or drop while training improves, this signals overfitting.

# 2. How can you use TensorBoard to detect overfitting?
Overfitting appears when training loss continues to decrease but validation loss increases. TensorBoard lets you visualize this divergence in real time.

# 3. What happens when you increase the number of epochs?
Initially, accuracy improves, but after a point, the model may start overfitting. Training accuracy keeps rising, while validation accuracy may flatten or fall.



