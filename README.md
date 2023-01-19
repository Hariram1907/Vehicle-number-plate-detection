# Vehicle number plate detection
 an automated vehicle number plate detection with gui

# Abstract

In today’s world with the increasing number of vehicles day by day it’s not possible to manually keep a record of the entire vehicle.With the increasing number of vehicles in today’s world it’s not possible to manually keep a record of the entire vehicle. There need to be a man standing 24*7 to note down the number. It’s a time consuming process and requires manpower. Furthermore the data stored manually is not readable after a long time. So to overcome all these limitations here we tried to develop a system which would automatically detect the number plate and store it in its database. With the development of this system it becomes easy to keep a record and use it whenever required. The main objective here is to design an efficient automatic vehicle identification system by using vehicle number plates. The system first would capture the vehicle's image as soon as the vehicle reached the security checking area. The captured images are then extracted by using the segmentation process. Optical character recognition is used to identify the characters. The obtained data is then compared with the data stored in their database. The system is implemented and simulated on MATLAB and performance is tested on real images. This type of system is widely used in Traffic control areas, tolling, parking area.etc. This system is mainly designed for the purpose of security. 

Keywords: Number Plate Recognition, Gray Processing, Image Acquisition, Image Binarization, Template Matching, Image to Text conversion, Easyocr, 
Introduction

# Problem Description :

The problem is to classify the various kinds of heavy vehicles from the web-camera. The classified vehicles have to be processed to capture the number plate of the vehicle. Then the captured number plate can be used to implement various systems with necessary functionalities such as registering the entry of the vehicle with vehicle registration number and time stamp value for maintaining the records of the vehicles entering into a place, etc.

# Scope & Objectives :

This type of system is widely used in Traffic control areas, tolling, parking area .etc
Can be used to register the number of vehicles entering a building or places like Shopping Malls, theatres, Institutions, Companies, etc.
Can also be used for monitoring the vehicles crossing the street, houses, roads.





# Work / activities carried out:

# Methodology adopted and workflow : 

Here is the methodology which have been followed to implement the solution for the problem discussed.

# Video from the web camera : 

Selecting the video file from the web camera video recordings.
Also can directly choose web camera video streaming.


# Capturing vehicles from video

Searching every frame of the video for the vehicles using the yolo v5 trained model for the vehicle detection.
A border box is drawn on the vehicles captured.
The coordinates of the box drawn will be retrieved.


# Classification of vehicles on video


# Cropping captured vehicles

The image of the vehicle is cropped from the frame of the video by using coordinates retrieved.
The image will be directed to the processing part.



# Processing cropped images
	
The image cropped from the video frame is converted to gray scale and searches for the rectangular part with text in it.
Then the rectangular border is drawn around the number plate.


# Processing the vehicle classified


# Cropping rectangular number plate

The coordinates of the border drawn around the rectangular number plate is collected.
The number plate part is cropped from the image of the vehicle by using the coordinates collected.



# Reading text from cropped plate

The number plate cropped image is used to find out the text.
Easy-Ocr is used to read the text from the number plate image.
It is displayed in the GUI.

# Number Plate image & text recognised


# Number Plate Registration

The text read from the image is displayed in the GUI
An excel sheet will be generated with the type of vehicle, Date, Time, Vehicle registration number.
The count of different types of vehicles is also displayed on the GUI.
The GUI also provides the facility of viewing the excel sheet within a small frame.

# Final result


# Result : 
 
This system can be very useful for recording the entry of vehicles into any institutions, hospitals, Shopping malls, etc.




