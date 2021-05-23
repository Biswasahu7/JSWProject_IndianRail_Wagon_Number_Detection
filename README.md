# JSWProject_IndianRail_Wagon_Number_Detection
This is one compouter vision project to our client JSW to detect Indian Railway wagon number. 
We have used yolov3 object detection transfer learning to achive our target. We have trained more then one million images to reach the acccuracy.

There are more then 6 object we have detected in this model.

1. Indian Railway Engine.
2. JSW Engine.
3. Wagon
4. Wagon type.
5. Coupling.
6. code

For each object we have taken image based on the light condition. Initial model we have trained only 1000 images for each object. 
According to the performance of the each model we have done some experiment based on that we have taken decision to reach the target.

First we need to detect Indian Railway engine, once it detect then our model logic will start working.
Model has to detect code image from wagon that code image has to pass the OCR to get 11 digit number from the image.
Once we will get number from model we need match with SAP.
If code has matched then we need to insert the code to JSW SQL database.
