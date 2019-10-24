# Cascade-Mask-RCNN
Cascade Mask R-CNN for object detection and instance segmentation on Keras and TensorFlow, based on matterport mrcnn.

This repository is based on matterport's Mask RCNN,  All codes are the same as matterport except 'mrcnn/model.py',  I add my cascade architecture  into this file . Therefore,  the usage methods are also the same as the existing Mask RCNN work , which based on matterport from GitHub or  blogs.   

## Useage

**All you need to do is replace the 'mrcnn/model.py'  to the original file** 

## Reference

According to the paper, I use the (c) architecture written by the author.

![1](https://github.com/anonymoussss/Cascade-Mask-RCNN/blob/master/assets/1.png?raw=true)

“I” is input image, “conv” backbone convolutions, “pool” region-wise feature extraction, “H”
network head, “B” bounding box, and “C” classification. “B0” is proposals in all architectures.“S” denotes a segmentation branch.

## Result

For simplicity, I use a small carplate datasets to train this model, so I can finish training in just a few hours, and it's also convenient to my debug . For instance,  "mrcnn3_bbox_loss" below means this loss come from the stage3 ( in figure (c) above)

![2](https://github.com/anonymoussss/Cascade-Mask-RCNN/blob/master/assets/2.png?raw=true)

**some detection results** 

![3](https://github.com/anonymoussss/Cascade-Mask-RCNN/blob/master/assets/3.png?raw=true)

![4](https://github.com/anonymoussss/Cascade-Mask-RCNN/blob/master/assets/4.png?raw=true)

## Last words

Implemented code is not stable during training, especially little datasets.  Maybe I haven't understand the paper  completely  now.  I haven't find better solution, If you have better idea, welcome correction！

