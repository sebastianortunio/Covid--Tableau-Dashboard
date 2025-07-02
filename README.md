# DNN IRIS – Classifying Flowers with Deep Learning

**Author:** Sebastian Ortuno  
---

This project builds a deep learning model to identify different types of iris flowers using their petal and sepal measurements. The data is cleaned and prepared so the model can learn properly, and the flower types are converted into a format the model can understand. The model uses several layers to learn patterns and decide which species each flower belongs to.

The model is trained over many rounds (epochs), using part of the data to check its accuracy as it learns. At the end, the model’s accuracy is measured, and the training progress is shown in charts. This project shows how a basic deep learning model can solve a simple classification problem step by step.

---
## Requirements

- R
- keras package
- tensorflow package

---
## How it works

1. **Load the libraries**  
   The project uses Keras and TensorFlow for building and training the model.

![image](https://github.com/user-attachments/assets/e54fd749-74f4-4f06-b52c-785a6dfd1880)


2. **Prepare the dataset**  
   The Iris dataset is shuffled and normalized. The species labels are converted into one-hot encoded vectors for classification.

![image](https://github.com/user-attachments/assets/e61c7ab3-4ba6-4a18-b6ba-add9e8be4994)


3. **Build the model**  
   A sequential deep neural network is created with two hidden layers (using relu activation) and an output layer with softmax activation for three classes.

![image](https://github.com/user-attachments/assets/e8cb66ae-ff84-4a61-a51f-a38e49a4f6e8)

4. **Compile the model**  
   The model is compiled with categorical cross-entropy loss and the Adam optimizer.
   
![image](https://github.com/user-attachments/assets/e85882b3-620d-45a4-8ed4-4685e5007f10)

5. **Train the model**  
   The model is trained over 200 epochs with 30% of the data reserved for validation.
   
![image](https://github.com/user-attachments/assets/719c5866-324d-46bd-ab9a-77fe1e11772f)

7. **Evaluate performance**  
   The model was evaluated using the same dataset after training. It achieved **96% accuracy**, meaning it correctly classified most of the iris flowers. The evaluation also reported a low loss value of **0.0808**, indicating good performance on this simple classification task.
   
![image](https://github.com/user-attachments/assets/8c8a636f-de08-4df4-9717-f24dd25c15cd)


8. **Visualize training**  
   The plot below shows the training and validation performance over 200 epochs. 

- Even though we don't have much data on iris and DNN works with bigger datasets, the model achieved 96% accuracy with a low loss of 0.0808, meaning it predicted the class correctly most of the time with minimal error. This confirms that the model learned well and generalized properly on the validation data.
   
![image](https://github.com/user-attachments/assets/3d53fd94-fb9a-4c74-abf3-f5516e91abae)

![image](https://github.com/user-attachments/assets/e147a6de-e6c4-4961-8ec3-a89bec1f5325)

---

## Conclusion

This project demonstrates how a simple deep neural network can effectively classify iris flowers using just a few features. It highlights the key steps of data preparation, model building, training, and evaluation in a clear and straightforward way. This approach can be easily adapted for other classification tasks or datasets.

---

