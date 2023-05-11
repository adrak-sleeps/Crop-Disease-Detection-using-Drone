# Crop-Disease-Detection-using-Drone

In this project, our aim is to:
1. To make a crop disease detection algorithm by using images of crops taken from ground level/manually.
2. To further modify the algorithm to detect crop diseases using images similar to images taken by a drone.

Firstly, we have selected our dataset as PlantVillage and created 3 models: 
1. 3-layered CNN
2. VGG-19
3. ResNet-9

We checked the accuracy of each model on the Dataset, and they were:
1. 3-layered CNN - 81.7%
2. VGG-19 - 85.5%
3. ResNet-9 - 99.2%

We then tried to modify the PlantVillage dataset so that the images are similar to images of crops captured by a drone. To do so, we blurred and zoomed them. 
On blurring the dataset, ResNet-9 gave a validation accuracy of 53.5%.

To modify this accuracy, we tried to deblur the images using the SelfDeblur model. ResNet-9 gave a validation accuracy of 64.24% after deblurring.

We tried to run our model on PlantDoc dataset and it did not perform well.
We tried to synthesise some realistic images using a GAN and got a validation accuracy of 25%. 

We aim to further improve these accuracies.

## How to run the CNN/VGG-19/ResNet file?

1. Download and open the "Crop Disease Detection using __ " file in Google Colab.
2. Run all cells.
3. On prompt to upload files, upload the kaggle.json file provided above.
4. Rest of the cells will run sequentially and provide output in approx 30-45 mins.

