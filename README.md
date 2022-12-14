# Vehicle-Counting-and-Classification
Nowadays, many places are equipped with surveillance systems that combine AI with cameras, from government organizations to private facilities. These AI-based cameras help in many ways, and one of the main features is to count the number of vehicles. It can be used to count the number of vehicles passing by or entering any particular place. This project can be used in many areas like crowd counting, traffic management, vehicle number plate, sports, and many more.  The process is simple:

    Frame differencing,
    Image thresholding,
    Contour finding,
    Image dilation.

And finally, vehicle counting.

# Description -

The steps that are involved in the process of vehicle detection and counting are given as follows.  

**1.1 Input Video -**

In this type of processing typically needs input data provided by the computer vision system and acting as a vision sensor and providing a high-level information. Then the video frames which are captured by the surveillance cameras are given as an input video for vehicle detection and counting. 

**1.2 Background Registration -**

 The Background registration technique is used to construct a reliable background image from the accumulated frame difference information. The moving object region is seperated from that background region by comparing the current frame with the background image. In background registration, the history of the frame difference mask is considered in constructing and updating the background buffer. If a pixel is marked as changing in the frame difference mask, the corresponding value in the stationary map is cleared to zero. Otherwise, if the pixel is stationary the corresponding value is incremented by one. The value in the stationary map is indicate that the corresponding pixel has been not changing for how many consecutive frames. If the pixel is stationary for the past several frames, then the probability is high that it belongs to the background region.  
 
**1.3 Image Subtraction -**

Image subtraction or pixel subtraction are process where the digital numeric value one pixel or whole image are subtracted from another image. This is primarily done for one of two reasons levelling uneven sections of an image such as half an image having a shadow on it, or detecting changes between two images.  This detection of changes can be used to tell if something in the image move. In which the target is moving and would be in one place in one image, and another from an image one hour later and where using this technique would make the fixed stars in the background disappear leaving only the target. 
 
 ![image](https://user-images.githubusercontent.com/105040357/207526521-b3eaaf0a-c512-410a-af25-93c8d259417e.png)
 
Fig 1: Subtraction of image 

**1.4 Foreground Detection -**

Foreground detection is one of the major tasks in the field of computer vision and image processing whose aim is to detect changes in image sequences. Background subtraction is any technique which allows an image's foreground to be extracted for further processing (object recognition etc.). Foreground detection separates foreground from background based on these changes taking place in the fore ground. It is a set of techniques that typically analyse video sequences recorded in real time with a stationary camera. 
 
 ![image](https://user-images.githubusercontent.com/105040357/207526389-d8371c68-e473-43eb-8bdd-d231711c60fd.png)
 
**1.5 Image Segmentation -**


Image segmentation techniques are interested in segmenting out different parts of the image as per the region of interest. As videos are sequences of images, motion segmentation aims at decomposing a video in moving objects and background by segmenting the objects that undergo different motion patterns. The analysis of these spatial and temporal changes occurring in the image sequence by separating visual features from     the scenes into different groups lets us extract visual information. Each group corresponds to the motion of an object in the dynamic sequence. 

**1.6 Vehicle Detection -**

Vehicle detection is a technique used in computer vision and image processing. Multiple consecutive frames from a video are compared by various methods to determine if any moving object is detected. Moving objects detection has been used for wide range of applications like video surveillance, activity recognition, road condition monitoring, airport safety, monitoring of protection along marine border.  

![image](https://user-images.githubusercontent.com/105040357/207526601-53bfe082-51e5-4e96-95c6-39ca662538d8.png)

Fig 3: Detection of vehicles 
 
**1.7 Vehicle Counting -**

In counting step, a counter is used to store the sum value of them. A counter should count the vehicles which are passing in the specific direction. So, if any vehicle stops, move turn in any direction in detection zone which are not counted. In this technique, counting is according to the number of moving vehicles detected in the detection zone. 
