# YOLO v4 - SPC Board detection

## Introduction
This YOLO v4 model is made to detect patterns on the default SPC Board 3 for calibration of fish and invertebrate on board images (see Measuring Board 3 below)

![Board template](https://github.com/PacificCommunity/cfap-ai-models/blob/master/YOLO_v4/SPC_Board3/board3.png)

The patterns locations are used to compute homography between detected patterns and template position and reproject the original image.

![Detected template](https://github.com/PacificCommunity/cfap-ai-models/blob/master/YOLO_v4/SPC_Board3/output/board3.jpg)

T10 : centerX = 200, centerY+objHeight/2 = 49
T20 : centerX = 400, centerY+objHeight/2 = 49
T30 : centerX = 600, centerY+objHeight/2 = 49
T40 : centerX = 800, centerY+objHeight/2 = 49
T50 : centerX = 1000, centerY+objHeight/2 = 49
T60 : centerX = 1200, centerY+objHeight/2 = 49
T70 : centerX = 1400, centerY+objHeight/2 = 49
B10 : centerX = 200, centerY-objHeight/2 = 329
B20 : centerX = 400, centerY-objHeight/2 = 329
B30 : centerX = 600, centerY-objHeight/2 = 329
B40 : centerX = 800, centerY-objHeight/2 = 329
B50 : centerX = 1000, centerY-objHeight/2 = 329
B60 : centerX = 1200, centerY-objHeight/2 = 329
B70 : centerX = 1400, centerY-objHeight/2 = 329
T0 : centerX = 0, centerY+objHeight/2 = 49
T05 : centerX = 99, centerY-objHeight/2 = 46
T15 : centerX = 299, centerY-objHeight/2 = 46
T25 : centerX = 499, centerY-objHeight/2 = 46
T35 : centerX = 699, centerY-objHeight/2 = 46
T45 : centerX = 899, centerY-objHeight/2 = 46
T55 : centerX = 1099, centerY-objHeight/2 = 46
T65 : centerX = 1299, centerY-objHeight/2 = 46
B0 : centerX = 0, centerY-objHeight/2 = 329
B05 : centerX = 99, centerY+objHeight/2 = 332
B15 : centerX = 299, centerY+objHeight/2 = 332
B25 : centerX = 499, centerY+objHeight/2 = 332
B35 : centerX = 699, centerY+objHeight/2 = 332
B45 : centerX = 899, centerY+objHeight/2 = 332
B55 : centerX = 1099, centerY+objHeight/2 = 332
B65 : centerX = 1299, centerY+objHeight/2 = 332
