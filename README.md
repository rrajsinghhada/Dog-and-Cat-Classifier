# Dog-and-Cat-Classifier

## Goal

The objective was to develop a machine learning model that could accurately distinguish between dogs and cats using images as inputs.

## Data

To construct this classifier, I utilised over 10,000 randomly selected images of dogs and cats as input to train the model. These images were deliberately chosen to encompass various lighting conditions, enhancing the model's ability to generalise.

## Steps taken to imporove the Performace of the model
•To increase data diversity and improve generalization, I applied transformations such as shear range, zoom range, and horizontal flip to my dataset.

•Feature scaling was applied to each pixel of the images by dividing them by 255, ensuring they were within the range of 0 to 1.

•A smaller kernel size of 3x3 was utilized, as it efficiently captures local patterns, enabling the model to learn more intricate details.

•Dropout layers were introduced during training to randomly deactivate a certain percentage of neurons. This technique aids in preventing    overfitting and enhances the model's ability to generalize.

## Result
Accuracy - 95.14 % (training data) and 80.64 % (test data) 

## Setup

The execution of the code necessitates a Python environment.

Clone the project:

```
$ git clone https://github.com/rrajsinghhada/Dog-and-Cat-Classifier
$ cd Dog-and-Cat-Classifier
```

Create a virtual environment, activate and install python packages:

```
$ python -m venv venv
$ source venv/bin/activate
$ pip install -r requirements.txt
```
for windows
```
$ pip install tensorflow
```




## Run the notebook:
For testing the model on images 
```
$ jupyter notebook Dog_Cat_Classifier.ipynb
```
For training the model
```
$ jupyter notebook Train_Model_CNN.ipynb
```
