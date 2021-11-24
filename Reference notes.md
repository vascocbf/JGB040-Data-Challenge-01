# List of hyper-parameters, defenitions, and functions in template model

# Relevant libraries: 

- numpy (linear algebra, arrays, matrices etc)

- pytorch (Machine Learning models)

- pyplot (making plots and other visualizations)

- sklearn (ML only used for dataset split)

# General parameters:

- batch_size

- n_epochs    (iterations)

- train/test data set size ratio

- number of layers (and size) in neural network

- what type of layers

To choose the layers and their specific components we would need to
look into the data to have an insight and be able to make smart choices.

Further research in what layers are available in pytorch.nn and their characteristics.




# Model Layers: 

(elapsed time: 5 minutes)

In this model the forward pass passes by the 3 2D convolution layers, 
and then the output is "flattened" to 1 dimension
using 2 linear function layers.



- 2D Convolution layer:	
- https://pytorch.org/docs/stable/generated/torch.nn.Conv2d.html?highlight=nn%20conv2d#torch.nn.Conv2d

	- in_channels  (input size for this layer) (for the first one it is 1 because it recieves 1 image)*
	- out_channels (output size of this layer)
	- kernel_size  (size of kernel for convolution)
	- stride       ("step size")
	- activation function: ReLU
	- dropout: probablility

- Linear layer:
- https://pytorch.org/docs/stable/generated/torch.nn.Linear.html?highlight=linear#torch.nn.Linear

	- in_features (input size per sample)
	- out_features (output size per sample)
	- bias (is there or not a bias feature in model)


	