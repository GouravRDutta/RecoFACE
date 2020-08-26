## RecoFACE 
## Introduction
RecoFACE is a Face Recognition Application made in python using OpenCV.

It uses OpenCV for capturing and handling the images.\
It uses OpenCV Haar-Cascade Classifier to search for faces in the entire image.\
It uses OpenCV Local Binary Patterns Histograms (LBPH) LBPHFaceRecognizer model for feature extraction and learns from them.\
The learnt model is then saved in a yml file.\
LBPHFaceRecognizer is also used for the detection of the learnt faces.


## Requirements
1. face_recognition
2. dlib
3. OpenCV
4. PIL.Image
5. OS
6. Pandas

## File Structure

RecoFACE(folder)-\
--------facedata(folder) - folder which contain all the pictures captured through webcam\
--------facetrainer(folder) -\
----------------names.csv - CSV file which contains the names of the person for which model is trained.\
----------------trainer.yml - contains trained data\
--------Face-Recognition(real-time).ipynb - Jupyter notebook python file containing code.
  
    
## HOW TO USE

1. Training the faces\
       You have to press 1 for a new user.\
       Camera window opens.\
          Enter user name.\
          Enter user number.(should be continuous for now till update comes)\
          Press key r to capture the images by looking at the camera. \
            Your face should be aligned properly.\
            30 images will be captured and saved in the facedata folder.\
            Window will automatically get closed after capturing images.\
          You can also press key q to quit the camera window.\
       The model will then automatically train upon the images clicked and will 
       save the data in trainer.yml file inside facetrainer.\
       The model will save the names of the user in names.csv file.\
       It will then give info on number of faces trained.
2. Detecting the faces
       You have to press 2 to open the detection window.\
       Camera window opens.\
       The trained model will automatically detect if any faces on which it has been trained is
       present in the window.\
       If a face is detected. The predicted name and percentage of prediction will be displayed 
       along with a green square surrounding the face.\
       Press key q to quit the window.
3. Press 3 for exit.



## Thank You 
Give a star if you like the Repo.


