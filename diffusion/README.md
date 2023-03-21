# TASK 3

An unconditional diffusion model has been trained on 100 images, with the hyperparameters from the original paper (with the exception of the number of the noise step[1000 in the paper to 100 in this case]). The loss value shown is MSE

The resulting images appear with a red background, instead of a blue one. This is a common issue with unconditional diffusion models. Since the model has no context about what the image should contain, it will often drift towards generating high frequency noise and random colors, rather than preserving the original background color.

To fix this, these are some of the possible solutions that can be used to improve the performance(not implemented because of time constraint):
- Injecting the original image as context
- Adding a color consistency loss
- Using a conditional model

