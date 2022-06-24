training
논문용 train:valid = valid외: 각 subject의 emo7장

training_0.99대0.01대1장
 - test 1장 빼고
 - valid용 1장빼고 학습 
 - train:valid:test = 0.99:0.01(1장):1장
 
 
 
ResNet152 학습환경 (동일하게 학습함)

 Parameters    60 Million
FLOPs     12 Billion
File Size    230.34 MB
Training Data  ImageNet
Training Resources      8x NVIDIA V100 GPUs

Training Techniques     Weight Decay, SGD with Momentum

Architecture:	1x1 Convolution, Bottleneck Residual Block, Batch Normalization, Convolution, Global Average Pooling, Residual Block, Residual Connection, ReLU, Max Pooling, Softmax

ID	resnet152
LR	0.1
Epochs	90
LR Gamma	0.1
Momentum	0.9
Batch Size	32
LR Step Size	30
Weight Decay	0.0001






MODEL	TOP 1 ACCURACY	TOP 5 ACCURACY
ResNet-152	78.31%	94.06%
ResNet-101	77.37%	93.56%
ResNet-50	76.15%	92.87%
ResNet-34	73.3%	91.42%
ResNet-18	69.76%	89.08%


https://paperswithcode.com/lib/torchvision/resnet
