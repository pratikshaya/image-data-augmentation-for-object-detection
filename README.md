# image-data-augmentation-for-object-detection
## Image Data augmentation and parsing into an XML file in Pascal-VOC format for object detection

Object detection in images is a hot topic in current research scenario and can be broken down into a wide range of applications like agriculture, security, surveillance, automated vehicle systems, and machine inception. Various methods of object detection algorithm from region-based CNN (R-CNN) to Faster R - CNN and YOLO to SSD have been established until today. But All these algorithms need a lot of training data along with ground truth bounding box. So, today I am going to explain about different image data augmentation technique and how to deal with change in the bounding box coordinate of the object in augmented data. After reading and implementing this blog, you can get the rich amount of augmented image as well as its XML file in Pascal-VOC format.


## Augmented method: (augmentation.py)
There are a vast number of augmentation technique in image processing. But I am only going to use PCA color augmentation, horizontal flip, vertical flip, rotation in 90, 180 and 270 degrees.

data_path and xml_path is the input image and xml annotation file of original data. input image is just a .jpg file and annotation file is .XML file in Pascal-VOC format. img_path is the path for augmented data that you will get after running this code. And out_path is .txt file that will contain the bounding box of ground truth object for augmented data. Inside .txt file of out_path you will get six values of image name, xmin, ymin, xmax, ymax and class in separate line.
After running the augmentation.py, you will get bunch of augmented image and the bounding box coordinates value of each object of augmented image in .txt format as below. Remember, if the image has multiple bounding box then it will save in different line as marked by red line below. The image name is same but the value of bounding box coordinates is different.
![a](https://user-images.githubusercontent.com/26374302/60764236-0684a780-a0c1-11e9-8e4b-ad80e93cac4e.png)
