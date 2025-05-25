### HOME ASSIGNMENT1

 # Overview
This project includes 3 TensorFlow tasks:
1. Tensor Manipulations & Reshaping
2. Loss Functions Comparison
3. Training a Neural Network with TensorBoard

 # Contents
- `tensor_manipulation.ipynb` – Tensor reshaping and broadcasting.
- `loss_functions.ipynb` – MSE vs Cross Entropy loss comparison.
- `mnist_tensorboard.ipynb` – MNIST model training with TensorBoard logging.

 # Student Info
- **Name: Vaishnavi Gopi** 
- **Student ID: 700754518**  
- **Course: Neural Networksand Deep Learning**
   
  

## 📽️ Demo Video
Link: [Insert Google Drive or YouTube video link here]

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



