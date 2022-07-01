# YOLO v4 - SPC Mat 1 detection

## Introduction
This YOLO v4 model is made to detect patterns on the default SPC Mat 1 for calibration of fish and invertebrates on SPC mat model 1 (see template below)

| ![Mat1 template](./mat1.png) |
|-|

The patterns locations are used to compute homography between detected patterns and template position and reproject the original image.


### Template mapping coordinates

* 

## Usage
1. Install AlexeyAB [darknet](https://github.com/AlexeyAB/darknet) implementation of Yolo v4
2. Copy cfg, data, model and samples folders to darknet installation folder
3. Run darket.exe from darknet installation folder

`darknet.exe detector test data/mat1.data cfg/yolov4-mat1.cfg model/yolov4-mat1_last.weights samples/fishes_on_mat1.jpg`

## Acknowledgements

This work conducted by the [Coastal Fisheries and Aquaculture Programme](https://fame.spc.int) of the [Pacific Community](https://www.spc.int), and funded by the Australian Department of Foreign Affairs and Trade (DFAT) and Pacific-European Union (EU) Marine Partnership (PEUMP) programme

## How to cite

Magron, Franck (2022) SPC Mat 1 Yolo v4 Model 1.0. https://github.com/PacificCommunity/cfap-ai-models/tree/master/YOLO_v4/SPC_Mat1. Pacific Community, Noumea.


