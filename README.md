# Object-Detection
Object detection with Detectron2

This project consists of three parts

1. Using COCO Keypoint Person Detector model with a ResNet50-FPN base network, which is trained to detect human silhouettes, to detect as many silhouettes of people in the test image as possible.

2. Repeat the above procedure, but with the Mask R-CNN model with ResNet50-FPN backbone, to detect both people as well as other objects in the scene.

3. Balloons in the test image are not being properly detected in either model. This is because the COCO dataset used to train the above models does not contain
balloons. Train a balloon detector using the (fine-tuning) balloon image dataset. Test it on the original test image to identify all the balloons
