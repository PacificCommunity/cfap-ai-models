# YOLO v4 - Survey photo types

## Introduction
This YOLO v4 model is made to detect the photo type and orientation and is the first step of image processing chain, before image calibration.

### Orientation

* *_R090 indicates the image is rotated right by 90°
* *_R180 indicates the image is rotated by 180°
* *_R270 indicates the image is rotated left by 90°

### Photo types

* FishesOnPathway12x8Mat (_R000/_R090)
* FishesOnPathway16x12Mat(_R000/_R090)
* FishesOnSpcMat1 (_R000/_R090/_R180/_R270)
* FishOnCalibratedBoard2 (_R000/_R090/_R180/_R270)
* FishOnCalibratedBoard3 (_R000/_R090/_R180/_R270)
* FishOnUncalibratedBoard (_R000/_R090/_R180/_R270)
* InvertOnCalibratedBoard2 (_R000/_R090/_R180/_R270)
* InvertOnCalibratedBoard3 (_R000/_R090/_R180/_R270)
* InvertOnUncalibratedBoard (_R000/_R090/_R180/_R270)
* InvertsOnSpcMat1 (_R000/_R090/_R180/_R270)
* Other (_R000)
* ScaleOnly (_R000/_R090/_R180/_R270)

### Notes
The detection of photo type rely on the dataset used for training. The current model might not be able to differentiate invertebrates on mat from fishes on mat for types of invertebrates not present in the training dataset for example.

## Usage
1. Install AlexeyAB [darknet](https://github.com/AlexeyAB/darknet) implementation of Yolo v4
2. Copy cfg, data, model and samples folders to darknet installation folder
3. Run darket.exe from darknet installation folder

`darknet.exe detector test data/survey_photo_types.data cfg/yolov4-survey_photo_types.cfg model/yolov4-survey_photo_types_last.weights samples/fish_on_board1.jpg`

## Acknowledgements

This work conducted by the [Coastal Fisheries and Aquaculture Programme](https://fame.spc.int) of the [Pacific Community](https://www.spc.int), and funded by the Australian Department of Foreign Affairs and Trade (DFAT) and Pacific-European Union (EU) Marine Partnership (PEUMP) programme

## How to cite

Magron, Franck (2022) Survey photo types Yolo v4 Model 1.0. https://github.com/PacificCommunity/cfap-ai-models/tree/master/YOLO_v4/SurveyPhotoTypes. Pacific Community, Noumea.


