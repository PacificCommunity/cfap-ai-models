# SPC CFAP Neural Network Models 

## Introduction

The [Coastal Fisheries and Aquaculture Programme](https://fame.spc.int) of the [Pacific Community](https://www.spc.int) develops neural network models for the analysis of fish and invertebrates pictures taken as part of market & landing surveys.

This repository contains the main models that are used as part of a image processing chain to calibrate images, detect, measure and identify specimens. Most detection models are based on YOLO v4, but we also use Detectron 2 PointRend for contouring and ResNet-101 for classifiers.

## Models
* [YOLO v4 - Survey photo types](./YOLO_v4/SurveyPhotoTypes)
* [YOLO v4 - SPC Board 3 detection](./YOLO_v4/SPC_Board3)
* [YOLO v4 - SPC Mat 1 detection](./YOLO_v4/SPC_Mat1)

## License
This work is licensed under Creative Commons Attribution-Non Commercial 4.0 license (CC BY-NC 4.0)

## Acknowledgements

This work has been funded by the Australian Department of Foreign Affairs and Trade (DFAT), European Union through Pacific-European Union (EU) Marine Partnership (PEUMP) programme and Australian Center for International Agricultural Research (ACIAR) through Australian National Centre for Ocean Resources and Security (ANCORS) Pathways 2 project



