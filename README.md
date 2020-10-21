# Mediclada

## Overview
Mediclada is a web app for predicting skin diseases particularly to help rural citizens of India who have \
limited access to Healthcare Services. For now it can predict upto 28 most commonly occuring skin diseases in rural India.\
Built with simplicity in mind, Mediclada uses resnet34 with the fast.ai library and is trained for 100 epochs on a custom image \
dataset of 28 different classes. The model has an amazing accuracy of 98% and has been deployed using Streamlit.

## Language
The whole project is written in Python3

## Dependencies 
Fast.ai (version : 1.0.61 ) \
Numpy \
Pytorch (version : 1.4.0 ) \
Pickle (version : 4.0 ) \
Streamlit (version 0.69.1) 

## Installation and Usage

To run the whole training process, first install all the dependencies and the dataset. Mention the path of the dataset \
in the `path = Path('C:/Dataset')` cell and run all the remaining cells to complete the training. Don't forget to save the \
model in the end. 

You can directly download the weights from this link (https://www.dropbox.com/s/dztcmi4x82m0xq1/export.pkl?dl=0) and run the code for the Web App \
or use the model you saved after training. Mention the path of the downloaded weights in the `learn = load_learner('C:/weights-file')`

## Working
![](walkthrough.gif)

Go to the website and upload an image (the option of clicking pictures is also available on smartphones). \
The Model then provides the Disease Prediction along with the common symptoms of the disease. 


## Disclaimer
1) The Images must be in .jpg or .jpeg format. 
2) The prediction may not be 100% accurate. Please consult a doctor for further information before taking any medication. 
3) Attaching a faulty/unclear image may result in wrong prediction or no prediction at all.
4) The files will be updated as more and more diseases get added. 
