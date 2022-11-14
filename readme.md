
# Traffic light classification Algorithm

* This is an algorithm for a convolutional neural network used for classifying traffic signs on the road.

## Architecture

```
Model: "sequential_9"
_________________________________________________________________
 Layer (type)                Output Shape              Param #   
=================================================================
 conv2d_17 (Conv2D)          (None, 21, 21, 32)        896       
                                                                 
 activation_27 (Activation)  (None, 21, 21, 32)        0         
                                                                 
 max_pooling2d_17 (MaxPoolin  (None, 10, 10, 32)       0         
 g2D)                                                            
                                                                 
 conv2d_18 (Conv2D)          (None, 3, 3, 64)          18496     
                                                                 
 activation_28 (Activation)  (None, 3, 3, 64)          0         
                                                                 
 max_pooling2d_18 (MaxPoolin  (None, 1, 1, 64)         0         
 g2D)                                                            
                                                                 
 flatten_5 (Flatten)         (None, 64)                0         
                                                                 
 dense_10 (Dense)            (None, 64)                4160      
                                                                 
 activation_29 (Activation)  (None, 64)                0         
                                                                 
 dropout_5 (Dropout)         (None, 64)                0         
                                                                 
 dense_11 (Dense)            (None, 1)                 65        
                                                                 
 activation_30 (Activation)  (None, 1)                 0         
                                                                 
=================================================================
Total params: 23,617
Trainable params: 23,617
Non-trainable params: 0
_________________________________________________________________

```

## Training and Testing set

* This model was trained and tested using the traffic lights dataset from Kaggle. Some of the images were augmented in order to better represent the real world scenarios.

## Results

* With this model, I was able to obtain an accuracy of 100% on the test set.
