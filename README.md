# Deep-learning-approaches-on-defect-detection-in-high-resolu-tion-aerial-images-of-insulators
The project of Deep learning approaches on defect detection in high resolu-tion aerial images of insulators
```
By detecting the defect location in high-resolution insulator images collected by un-manned aerial vehicle (UAV) in various environments, the occurrence of power failure can be timely detected and the caused economic loss can be reduced. However, the accuracies of existing detection methods are greatly limited by the complex background interference and small target detection. To solve this problem, two deep learning methods based on Faster R-CNN (faster re-gion-based convolutional neural network) are proposed in this project, namely Exact R-CNN (exact region-based convolutional neural network) and CME-CNN (cascade the mask extraction and exact region-based convolutional neural network). Firstly, we proposed an Exact R-CNN based on a series of advanced techniques including FPN (feature pyramid network), cascade regression, and GIoU (generalized intersection over union). RoI Align (region of interest align) is introduced to re-place RoI pooling (region of interest pooling) to address the misalignment problem, and the depthwise separable convolution and linear bottleneck are introduced to reduce the computational burden. Secondly, a new pipeline is innovatively proposed to improve the performance of insulator defect detection, namely CME-CNN. In our proposed CME-CNN, an insulator mask image is firstly generated to eliminate the complex background by using an encoder-decoder mask extraction network, and then the Exact R-CNN is used to detect the insulator defects. The experimental results show that our proposed method can effectively detect insulator defects, and its accuracy is better than the examined mainstream target detection algorithms.
```
## 1.requirement
- Python 3
- Keras and TensorFlow. 
- numpy
- opencv

## 2.dataset
```
the dateset of insulator,include Defective_Insulators_images(288) and Normal_Insulators_images(108)
```

## 3.train

### 3.1 Modify the config.py configuration file
```
The dataset path in the configuration file is configured as its own path
```
### 3.2 Perform training
```
$ train.py
```

