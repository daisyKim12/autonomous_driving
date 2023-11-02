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



![](RackMultipart20231102-1-w8xtez_html_bbbe969e4a457c99.png)임의로 꼬깔을 이용한 track을 만든 후 유아용 자동차를 직접 움직여 가며 camera로 부터 들어오는 사진에 이동해야할 위치를 직접 찍어주었고 좌회전 우회전 및 직전 등의 DATASET을 약 4500장 수집하였다.

## Directory content

- ROAD FOLLOWING
    - road_following.zip
    - rf_data_collection.ipynb
    - rf_train_model.ipynb
    - rf_live_detection.ipynb
- OBJECT DETECTION
    - object_detection.zip

## Road Following code explanation


## Object Detection code explanation


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