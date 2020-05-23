# p and g global innovation
Detecting consumer product feedback using customers' reaction by using face expression as well doing customer segmentation based on age &amp; gender

The whole project is devided into 3 parts.
1) Face detection & Facial Landmark detection. (It will be used for next 2 steps)
2) Customers' face expression detection and stored the time for the further analysis and graph representation.
3) Customers' age and gender detection for customers' segmentation analysis for the product.

Let's understand the project structure. 
1-facial-points-realtime
2-emotion-realtime
3-AgeGender-realtime
master.py

we need to run the master.py file to run the whole project:

python master.py

To understand each files seprately, we need to run this one by one like this

1) Face detection & Facial Landmark detection. (It will be used for next 2 steps)
cd 1-facial-points-realtime/
and run the file
python facial_landmarks.py --shape-predictor shape_predictor_68_face_landmarks.dat

2) Customers' face expression detection and stored the time for the further analysis and graph representation.
cd 2-emotion-realtime
and run the file
python emotion_detector.py --cascade haarcascade_frontalface_default.xml --model checkpoints/epoch_75.hdf5

3) Customers' age and gender detection for customers' segmentation analysis for the product.
cd 3-AgeGender-realtime
python AgeGender.py

Thank You.

