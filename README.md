# Stroma Vision Task

We are building a computer vision pipeline for a nuts-and-bolts manufacturer. For Dataset operations, preprocessing operations were carried out with the notebook locally. For Training and Testing, object detection with Yolov8 and tracking with ByteTrack & Supervision are performed in Colab.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

## Prerequisites

What things you need to install the software and how to install them

## Installing

### Create Python Virtual Environments

Since notebook will be used in local for dataset operations, virtual environment is created with the following commands.

```bash
conda create --name stroma-vision python=3.10.6
pip install -r requirements.txt
```

### Run

```bash
git clone https://github.com/Tolgaisikp/stroma-vision-task.git
```

You can convert the data given coco annotation to yolo annotation by running the first 3 notebooks above. to mention the above notebooks respectively

* 1-extract-image.ipynb : This file contains functions to extract pictures from train test and val videos in the challenge folder.
* 2-coco-to-yolov8.ipynb : This file converts the dataset which is coco annotation to yolo annotation with pylabel importer and creates the dataset.yaml file.
* 3-delete-empty-img.ipynb : This file deletes the empty labels by looking at the sizes of the labels created in 2-coco-to-yolov8 and accordingly deletes the images of the deleted labels.
* 4-custom-yolov8-train_and_test.ipynb : This file contains the Google Drive link of the dataset for Training and Testing, the Github link of the code and the markdown containing the Colab link.

## Built With

* [Colab](https://colab.research.google.com/drive/1xVMnB-3uSYEbZE7Nb0BSokJcuGGZIPMC?usp=sharing) - GPU powered Jupyer Notebook
* [YoloV8](https://github.com/ultralytics/ultralytics) - YoloV8 Github link
* [Dataset](https://drive.google.com/file/d/1j8RAxBHwEI1zanmblq0RuQiFDGLHN-ig/view?usp=sharing) - Latest version of the Dataset

## Authors

**Tolga Işık** - [Tolgaisikp](https://github.com/Tolgaisikp)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
