## Data Science Reflection 3

### Deep Learning Object Detection and Disney's Content Genome

As previously discussed, Disney has created a Content Genome built within Disney’s Direct-to-Consumer & International Organization (DTCI). By creating an archive of Disney 
content and animations, both animators and consumers will benefit. Using both traditional and more recent methods of object detection, DTCI has created a way for animators 
to search and emulate past animations. Through the course of research and development, engineers ultimately used Faster-RCNN Object Detection to recognize both live action
and animated features.

It is important to make the distinction between image classification and object detection when working with complex recognition methods. **Image classification** is used to
classify and label the most dominant object of an image. When the input is presented to a neural network, a single class label is applied appropriately. **Object detection**,
on the other hand, utilizes multiple bounding boxes within a single image and applies a label for each box along with the probability score in terms of a percent. While image 
classification can be useful in a rudimentary setting, object detection is often more robust for the uses of developers. 

The more traditional approach to object detection utilizes HOG+SVM and was first used for the Content Genome. This method uses **sliding windows** to move left-to-right and 
top-to-bottom to identify objects in the scope of smaller sections of the image. In addition, an **image pyramid** is used to detect objects in varying scales. Neural networks 
stemming form image classification give more background and context to the input. While this is a simpler method, it can save time and effort if it is effective for its specific need. Unfortunately for Disney, this method was unsuccessful in properly identifying animated objects. 
Rather, DCTI worked with “Faster-RCNN Object Detection architecture trained over the COCO dataset” (Accardo et al., 2020). In this method, image classification is used as a 
**base network**, a pretrained set of data to classify the image dataset. The framework of the object detection, Faster RCNN, contains several parts including an anchor set, 
a Convolutional Neural Network, ROI, and RPN. An advantage to this method is that the network can be edited to replace less useful components of the network with more useful 
ones. DTCI took advantage of this when they added animations with solely objects rather than faces to the dataset. Overall, the deep learning object detection method that DCTI
used for their Content Genome proved to be more effective than traditional methods. As object detection is being applied to many different sectors of our modern world,
more complex methods of detection are needed to recognize a broader range of objects. 


#### References

Accardo, Anthony, et al. How Disney Uses PyTorch for Animated Character Recognition. 16 July 2020, medium.com/pytorch/how-disney-uses-pytorch-for-animated-character-
recognition-a1722a182627. 

Rosebrock, A. (2020, April 18). A Gentle guide to Deep Learning Object Detection. Retrieved October 16, 2020, from https://www.pyimagesearch.com/2018/05/14/a-gentle-
guide-to-deep-learning-object-detection/
