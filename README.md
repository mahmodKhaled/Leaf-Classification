# Leaf-Classification

## Dataset Description 
The dataset consists approximately 1,584 images of leaf specimens (16 samples each of 99 species) which have been converted to binary black leaves against white backgrounds. Three sets of features are also provided per image: a shape contiguous descriptor, an interior texture histogram, and a ﬁne-scale margin histogram. For each feature, a 64-attribute vector is given per leaf sample.

Note that of the original 100 species, we have eliminated one on account of incomplete associated data in the original dataset.

## Project Phases
### Phase1: Data Preparation
1. First, download the data file, load it, and 
   - Describe the data
   - Clean the data 
   - Check the data for missing values or duplicates and carry out proper correction methods
   - Visualize the data using proper visualization methods. 
   - Draw some of the images 
   - Carry out required correlation analysis
2. divide the data into a training and test set using approximately 80% for training. 
3. Decide if you need to standardize the data, by computing the mean and standard deviation for each feature dimension using the training set only, then subtracting the 
mean and dividing by the stdev for each feature and each sample. 
4. Encode the labels

### Phase2: Training a neural network
In this project, we will need to implement a 3-layer MLP model (one input layer, one hidden layer with tanh activation and one output layer) which will be used to classify the data in Part I.
we also need to write the training function (training), and should explore the following hyperparameter settings:
- Batch size: Number of examples per training iteration. 
- Hidden size: Try using different number of hidden nodes in your model and compare the performances. 
- Dropout is an effective strategy to defend against overfitting. Adding a dropout layer after the hidden layer, and try using different dropout rate to compare the performances. 
- Optimizer: Try using different optimizers such as **SGD**, **Adam**, **RMSProp**. 
- Regularization (weight decay): L2 regularization can be specified by setting the 
weight_decay parameter in optimizer. Try using different regularization factor and check the performance. 
- Learning rate, Learning rate scheduler: Learning rate is key hyperparameter in model training, and you can gradually decreasing the learning rate to further improve your model. Try using different learning rate and different **learning rate scheduler** to compare the performance.
