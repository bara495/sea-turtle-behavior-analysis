# Sea Turtle Behavior Analysis

Entry point for the models, datasets, and (forthcoming) code behind our work on rehabilitation-tank
sea turtle behavior — breathing (head-out) event detection and within-tank mobility analysis,
comparing a turtle exposed to acoustic playbacks against a control turtle.

If you're here from the paper: this repo is the place to find everything needed to understand or
reproduce the results. Code is not yet published here — see "Status" below.

## Models

| Model | Description |
|---|---|
| [sea-turtle-breathing-resnet50](https://huggingface.co/marko-barisic/sea-turtle-breathing-resnet50) | ResNet50 binary classifier — detects whether a turtle's head is above the water surface (breathing) from overhead tank camera frames. |
| [sea-turtle-detection-yolov8](https://huggingface.co/marko-barisic/sea-turtle-detection-yolov8) | YOLOv8 detection/segmentation model — locates the turtle's body in each frame, used to derive tank-position centroids for the mobility analysis. |

## Datasets

| Dataset | Description |
|---|---|
| [sea-turtle-breathing](https://huggingface.co/datasets/marko-barisic/sea-turtle-breathing) | Labeled image dataset (breathing / not-breathing) used to train the breathing classifier. |
| [sea-turtle-behavior-data](https://huggingface.co/datasets/marko-barisic/sea-turtle-behavior-data) | Raw video recordings for both turtles, both experimental days. |
| [sea-turtle-assets](https://huggingface.co/datasets/marko-barisic/sea-turtle-assets) | Deployed model weights and the locked event-extraction configuration actually used to produce the paper's results. |

## Paper

*Citation / DOI to be added once available.*

## Status

This repo currently serves as a landing page linking the models and datasets above. Pipeline code
(detection, breathing classification, and the mobility/heatmap analysis) will be added here.

## Authors

- **Marko Barišić** — University of Zagreb, FER, Laboratory for Underwater Systems and Technologies (LABUST)
- **Roee Diamant** — University of Haifa
