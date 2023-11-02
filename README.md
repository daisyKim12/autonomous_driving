# autonomous_driving
Creating a self-driving car by connecting a JETSON Nano board with a child-friendly car. I am designing and modifying artificial intelligence algorithms to implement autonomous driving for the car. I am also incorporating image recognition using YOLO, to stop the car on stop sign.

## ◆ SETUP

◇ HARDWARE SETUP

![](x/Screenshot%202023-11-02%20at%203.42.52%20PM.png)

- JETBOT setup   
![](x/Screenshot%202023-11-02%20at%203.42.17%20PM.png)   
- JETBOT & Car Motor setup   
![](x/Screenshot%202023-11-02%20at%203.42.25%20PM.png)   

◇ SOFTWARE SETUP
- SD card & connect using wifi  
![](x/Screenshot%202023-11-02%20at%203.42.35%20PM.png) ![](x/Screenshot%202023-11-02%20at%203.42.44%20PM.png)   

## Directory content

- ROAD FOLLOWING
    - road_following.zip
    - rf_data_collection.ipynb
    - rf_train_model.ipynb
    - rf_live_detection.ipynb
- OBJECT DETECTION
    - object_detection.zip

## Road Following code explanation
We transfered resnet18 to use it as a regression model.
Training data was image with x,y coordinates as a label. x,y coordinate indicates where to stir the vehicle.
We made 3000 images as a dataset. 10% of the dataset as test dataset and 90% as training dataset.

## Object Detection
We use Yolo v5 to detect stop sign to stop the vehicle.

## ◆ ROAD FOLLOWING: DATA SET

◇ Attempt1: data distribution

| total data | 1800 |
| --- | --- |
| straight | 800 |
| left | 600 |
| right | 400 |

◇ data sample   
![](x/Screenshot%202023-11-02%20at%203.43.33%20PM.png)
![](x/Screenshot%202023-11-02%20at%203.43.37%20PM.png)
![](x/Screenshot%202023-11-02%20at%203.43.41%20PM.png)

◇ Attempt2: data distribution

| total data | 1800 + 1200 |
| --- | --- |
| straight | 1000장 |
| left | 1000장 |
| right | 1000장 |

◇ data sample   
![](x/Screenshot%202023-11-02%20at%203.44.37%20PM.png)

## ◆ ROAD FOLLOWING: DATA SET 3

◇ Attempt3: data distribution

| total data | 1800 + 1200 + 1500 |
| --- | --- |
| straight | 1000 + 1500 |
| left | 1000 + 0 |
| right | 1000 + 0 |

◇ data sample   
![](x/Screenshot%202023-11-02%20at%203.44.47%20PM.png)