# CL_SPP

## implementation
In this repository, CL_SPP are implemented by tensorflow 1.3.0，Python 3.5，cuda 8.0 and openCV 3.3.1.

## Augmentation 
In the experiment of incremental learning Caltech-101, we used data augmentation as follow:
|method         |setting |
|----------     |------ |
|rotation       |90 degree |
|random resize  |[224，224，3] |
|mirror         |random |
|flip           |random |

## note: 
1. To quickly search the best hyper-parameters, we used a greedy search strategy, we firstly adjusted the optimal learning rate and then random search the optimal lambda.
2. The experiments on split-MNIST and CIFAR10/SVHN/NOT-MNIST/STL-10 were implemented on original datasets with a size of 32*32.
3. Batch size is 128. All experiments were performed on a single GTX1080ti.
4. The original model on experiment of Caltech-101 is resnet18.

## training 
In this repository, we present 3 experiments on SPP, including split-MNIST,CIFAR10/SVHN/NOT-MNIST/STL-10 and Caltech-101. Each folder contains SPP and other approaches of baseline.
You can get the result of SPP and other 8 methods just run the script with the corresponding name.


## Citation 
If you use SPP in your research, please cite the paper:




