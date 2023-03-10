# Decentralized-Machine-Learning-

## Abstract: 

Decentralized Machine Learning is the distributed training of an ML model on more than 
one device. It reduces the computational load on a device by distributing the centralized 
training models over many devices. Distributed training models, in contrast to centralized 
systems, utilize local datasets in a distributed network to ensure the confidentiality of user 
data. Large datasets boost accuracy, according to research, but training them takes a long 
time and a lot of computational power. As a result, decentralized machine learning is 
advantageous for applications that demand huge datasets, such as 3D scene generation, 
high image classification, and so on. There are two aspects of the problem: (1) Deploying 
ML models on edge devices and (2) distributed training of ML models. So our initial 
approach is to assume that both data and model are centralized and we need to 
decentralize the model by distributing the data across each device. Each device will be 
trained individually and will compute the model gradients. These gradients will be 
aggregated by the master/central server. The results of this approach were not satisfying 
as we observed disappointing results. After reviewing the recent work, we are working on 
devising the algorithm which will assign some initial weights to each client‘s gradients. 
Our initial investigation is that these effects impact the results strongly due to bias-shuffling of samples while distributing the dataset among the client/devices. So we can 
sum up the required research and development process as it involves (1) sending of the 
distributed datasets to the local devices (2) parallel training of each device using local 
datasets and (3) updating the hyper-parameters of local training models using dynamic 
model averaging
