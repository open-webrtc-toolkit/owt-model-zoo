# Selfie segmentation

These models are converted from https://github.com/PINTO0309/PINTO_model_zoo/blob/main/082_MediaPipe_Meet_Segmentation, which is from Google MediaPipe. See [Model Card-Meet Segmentation.pdf](https://github.com/PINTO0309/PINTO_model_zoo/blob/main/082_MediaPipe_Meet_Segmentation/Model.Card-Meet.Segmentation.pdf) for original model details.

## Input

A tensor of shape 1 x 3 x H x W and data type of 32-bit float ranging from [0, 1], representing a three-channel RGB image of width H and height W whose value is divided by 255.

H=144 and W=256 for the model in 144x256 directory.

## Output

A tensor of shape 1 x H x W and data type of 8-bit unsigned integer ranging from [0, 255], representing the probability of the corresponding pixel belonging to human, multiplied by 255 and truncated into integer.

H=144 and W=256 for the model in 144x256 directory.

