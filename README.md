# image-data-augmentation-for-object-detection
Image Data augmentation and parsing into an XML file in Pascal-VOC format for object detection

Object detection in images is a hot topic in current research scenario and can be broken down into a wide range of applications like agriculture, security, surveillance, automated vehicle systems, and machine inception. Various methods of object detection algorithm from region-based CNN (R-CNN) to Faster R - CNN and YOLO to SSD have been established until today. But All these algorithms need a lot of training data along with ground truth bounding box. So, today I am going to explain about different image data augmentation technique and how to deal with change in the bounding box coordinate of the object in augmented data. After reading and implementing this blog, you can get the rich amount of augmented image as well as its XML file in Pascal-VOC format.


#Augmented method: (augmentation.py)
