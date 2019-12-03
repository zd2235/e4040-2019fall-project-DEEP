# e4040-2019fall-project-DEEP

## Requirement:tensorflow 2.0

### Whole model built based on keras with existing tf.keras.layer.funcs,
### may be changed into tf.nn.layers for outside weight operations.

## Realized:
### 1. Mobile Net structure (with question of output size on the 9th depthwise separable  convolution).
### 2. Hyperparameter: width multiplier
### 3. Test training with CIFAR100 (50000,32,32,3)

## Remained:
### 1. ImageNet Dataset (N,224,224,3) acquisition
### 2. Hyperparameter: resolution multiplier (how to simply change input resolution?)
### 3. Unknown methods implementation:
###               RMSprop  --> how to use  asynchronous gradient descent?
###               convolution calculation: are tensorflow funcs GEMM funcs?
###               Depthwise conv --> how to reduce or cancel weight decay in depthwise filters?