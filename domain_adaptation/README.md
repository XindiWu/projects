# 3D Adversarial Domain Adaptation
3DADA is a deep learning based framework for subtomogam classification domain adaptation of Cellular Electron Cryo Tomography data

Please refer to our paper for more details:

R Lin, X Zeng, K Kitani, M Xu. "Adversarial domain adaptation for cross data source macromolecule *in situ*  structural classification in cellular electron cryo-tomograms"

To run the code, please follow these steps:
1. Data preparation: Our model is designed for 3D subtomogram data. To run the code, you need to prepare source and target data in size as (N,40,40,40) and Label in size as (N,). You can see our sample data for details. Other input data size may or may not need to modify the network structure to fit in. 
2. Hyperparameter choose: You need to pick up some hyper parameters such as batchsize and learning rate. You can use arguments to set up or just modify train.py for them.
3. Run train.py

Adversarial learning implemented in updater.py and models implemented in c3dmodels.py


## Key prerequisites
* [keras](https://keras.io/#installation)
* [tensorflow-gpu](https://www.tensorflow.org/install/)
* numpy
```
pip install numpy
```

* scipy
```
pip install scipy
```


## Installation 
```
git clone https://github.com/xulabs/projects.git
```


## Example dataset

http://xulab-gpu0.pc.cs.cmu.edu/190326-domain-adaptation-ismb--b7251f2e-500e-11e9-9a7e-5f79e91ebde5/DA_simulated.tar.gz
