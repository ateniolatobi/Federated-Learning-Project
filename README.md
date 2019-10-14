# Project - FEDERATED LEARNING ON THE MNIST DIGIT DATASET

## ABSTRACT

Federated Learning is a machine learning setting where the goal is to train a high-quality centralized model with training data distributed over a large number of clients each with unreliable and relatively slow network connections. We consider learning algorithms for this setting where on each round, each client independently computes an update to the current model based on its local data and communicates this update to a central server, where the client-side updates are aggregated to compute a new global model. The typical clients in this setting are mobile phones, and communication efficiency is of utmost importance. 



---



## Visualization of Federated learning across several devices



<img src="https://github.com/ateniolatobi/Federated-Learning-Project/blob/master/assets/fdl.png" width="100%">



## PROJECT DESCRIPTION

Federated learning involves the training of remote deep learning models across different devices before aggregating the weights learned from the remote devices into a central model. This is done in order to ensure that privacy is conserved across the remote devices by ensuring the central model has no access to the personal data of the remote devices involved and only has access to the weights of the remote models.    

- In this project, remote devices are not used but the process of training across remote models is simulated by dividing a dataset into various sub-datasets and then creating unique independent models for each sub-dataset.  
- A central model would be created which would have no access to the dataset but would only have access to the weights gotten from training the remote models anonymously.
- Virtual workers would be used from the Pysyft python package to simulate the Independent anonymous devices where the remote models would be stored.
The Independent anonymous models would be trained on their respective sub-datasets then the weights learned would be returned to a central model where they would be aggregated.  
- The process above ensures that the central model has no access to the actual sub-datasets but only has access to the weights gotten from training remote models across the sub-datasets. This ensures anonymously of the sub-databases thus conserving privacy and at the same time ensures the central model is accurate enough to make meaningful predictions.

---



## Tools Used

> The model was created and trained with PyTorch and the MNIST digit dataset was used to train the models.


- torch==1.1.0
- torchsummary==1.5.1
- torchtext==0.3.1
- torchvision==0.3.0
- syft==0.1.29a1
- numpy==1.16.4
- matplotlib==3.0.3




```

pip install torch

pip install syft

pip install pandas

pip install numpy 

pip install matplotlib

```



## References

1. [Federated Learning: Strategies for Improving Communication Efficiency](https://ai.google/research/pubs/pub45648)

2. [Secure and Private AI course Udacity](https://www.udacity.com/course/secure-and-private-ai--ud185)

3. [The New Dawn of AI: Federated Learning](https://towardsdatascience.com/the-new-dawn-of-ai-federated-learning-8ccd9ed7fc3a)

