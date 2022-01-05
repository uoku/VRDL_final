# RSNA Pneumonia Detection Challenge

## Hardware and sofeware
* Intel Core i7-8700k
* 16 GB RAM
* NVIDIA GeForce GTX 1070
* Windows 10 (Version 1803)
* Python 3.5.4
* CUDA 9.0
* cuDNN 7.0

## data preprocess

put all data from kaggle in data/

1.create `stage_2_train_images_png` dictionary

2.create `stage_2_test_images_png` dictionary

3.go to `preprocessing` dictionary

4.run `python dcm_2_png_train.py` and `python dcm_2_png_test.py`


## Train

Classification

1.go to `classification` dictionary

2.Run `python classifier_train.py` to train classifier (SPLIT_NUMBER to choose which one to train)


Bounding-Box Detection

1.go to `detection` dictionary

2.Run `python train_rsna.py` to train classifier (SPLIT_NUMBER to choose which one to train)


## Inference

1.go to `classification` dictionary

2.Run `python classifier_predict.py`

3.go to `detection` dictionary

4.Run `python predict_rsna.py`

5.run `python generate_final_prediction.py`


## best model

- [My awesome model](https://drive.google.com/file/d/1jdxkmAVYBW68IbTOwfrVSeEIQO8ZWHXU/view?usp=sharing) 

1.put weights in weights_classification in classification/weights

2.put weights in weights_detection in detection/weights

## Reference

https://github.com/erniechiew/kaggle_rsna_pneumonia_dancingbears
