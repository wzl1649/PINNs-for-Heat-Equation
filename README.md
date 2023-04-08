# PINNs-for-Heat-Equation
This is only created for learning purpose. I use Physical Informed Neural Networks( PINN) to train a model that approximate the solution of a given heat equation

What we want to solve is the standard heat equation
$$u_t = u_xx$$
in the region of [0,1]^{3} with B.C. uniformly zero and I.C.
$$u(x,y,0)= sin(\pi x)sin(\pi y)$$
The theortical solution is 
$$u(x,y,t) = e^{-2 \pi^{2} t} sin(\pi x)sin(\pi y)$$

## Further explanation on the uploaded files:
- "heat_test.ipynb" is the main code file, including the structure of the neural network and train step
- "plot_only.ipynb" is created to plot interative pictures since some packages used  donot consistent with my tensorflow version
- "Heat_PINN_weights.h5" is a h5 file storing the pretrained weights and bias, i.e. the coefficients of the neural network. You can use this to check the performance or to further optimize it
- "Predictions.npy" is save by numpy to transfer data generated by the model for ploting purpose

