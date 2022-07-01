# YOLO v4 - SPC Board 3 detection

## Introduction
This YOLO v4 model is made to detect patterns on the default SPC Board 3 for calibration of fish and invertebrates on measuring board images (see Measuring Board 3 template below)

![Board template](https://github.com/PacificCommunity/cfap-ai-models/blob/master/YOLO_v4/SPC_Board3/board3.png)

The patterns locations are used to compute homography between detected patterns and template position and reproject the original image.

![Detected template](https://github.com/PacificCommunity/cfap-ai-models/blob/master/YOLO_v4/SPC_Board3/output/board3.jpg)

### Template mapping coordinates

* T10 : centerX = 200, centerY+objHeight/2 = 49
* T20 : centerX = 400, centerY+objHeight/2 = 49
* T30 : centerX = 600, centerY+objHeight/2 = 49
* T40 : centerX = 800, centerY+objHeight/2 = 49
* T50 : centerX = 1000, centerY+objHeight/2 = 49
* T60 : centerX = 1200, centerY+objHeight/2 = 49
* T70 : centerX = 1400, centerY+objHeight/2 = 49
* B10 : centerX = 200, centerY-objHeight/2 = 329
* B20 : centerX = 400, centerY-objHeight/2 = 329
* B30 : centerX = 600, centerY-objHeight/2 = 329
* B40 : centerX = 800, centerY-objHeight/2 = 329
* B50 : centerX = 1000, centerY-objHeight/2 = 329
* B60 : centerX = 1200, centerY-objHeight/2 = 329
* B70 : centerX = 1400, centerY-objHeight/2 = 329
* T0 : centerX = 0, centerY+objHeight/2 = 49
* T05 : centerX = 99, centerY-objHeight/2 = 46
* T15 : centerX = 299, centerY-objHeight/2 = 46
* T25 : centerX = 499, centerY-objHeight/2 = 46
* T35 : centerX = 699, centerY-objHeight/2 = 46
* T45 : centerX = 899, centerY-objHeight/2 = 46
* T55 : centerX = 1099, centerY-objHeight/2 = 46
* T65 : centerX = 1299, centerY-objHeight/2 = 46
* B0 : centerX = 0, centerY-objHeight/2 = 329
* B05 : centerX = 99, centerY+objHeight/2 = 332
* B15 : centerX = 299, centerY+objHeight/2 = 332
* B25 : centerX = 499, centerY+objHeight/2 = 332
* B35 : centerX = 699, centerY+objHeight/2 = 332
* B45 : centerX = 899, centerY+objHeight/2 = 332
* B55 : centerX = 1099, centerY+objHeight/2 = 332
* B65 : centerX = 1299, centerY+objHeight/2 = 332

## Usage
1. Install AlexeyAB [darknet](https://github.com/AlexeyAB/darknet) implementation of Yolo v4
2. Copy cfg, data, model and samples folders to darknet installation folder
3. Run darket.exe from darknet installation folder

`darknet.exe detector test data/board3.data cfg/yolov4-board3.cfg model/yolov4-board3_last.weights samples/fish_on_board1.jpg`

## Acknowledgements

This work conducted by the [Coastal Fisheries and Aquaculture Programme](https://fame.spc.int) of the [Pacific Community](https://www.spc.int), and funded by the Australian Department of Foreign Affairs and Trade (DFAT) and Pacific-European Union (EU) Marine Partnership (PEUMP) programme

## How to cite

Magron, Franck (2022) SPC Measuring Board 3 Yolo v4 Model 1.0. https://github.com/PacificCommunity/cfap-ai-models/tree/master/YOLO_v4/SPC_Board3. Pacific Community, Noumea.


