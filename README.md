# SATELLITE IMAGE SEMANTIC SEGMENTATION
This project is a part of a Kaggle cometition in Deep Learning course at CentraleSupelec and is carried out with my team member i.e. Vanshika Sharma
## Project description
The task was to employ deep learning to segment and classify the objects (26 labels) in the satellite images. The dataset comprises 374 images (3x3000x4000) of residential neighborhoods in Houston after the hurricane Harvey. 299 out of the total images have corresponding masks which were used for training deep learning models. The competition requires the submission of the masks for the remaining 75 images. The evaluation metric is dice score. A snapshot of the images and provided masks are as followed:

![image](https://user-images.githubusercontent.com/85484281/213866548-7f770301-9f7a-466f-bfee-c6e3004aee18.png)
## Pre-processing and exploration
After the exploration, we decided to:
- oversampled by creating additional 84 images to address the unbalanced labels (spliting the images containing under-represented labels into 4)

![image](https://user-images.githubusercontent.com/85484281/213866790-ceee17e1-1b0a-439f-bb58-a5a88237b0a7.png)

*Label list = {
'Property Roof': 0,
 'Secondary Structure': 1,
 'Swimming Pool': 2,
 'Vehicle': 3,
 'Grass': 4,
 'Trees / Shrubs': 5,
 'Solar Panels': 6,
 'Chimney': 7,
 'Street Light': 8,
 'Window': 9,
 'Satellite Antenna': 10,
 'Garbage Bins': 11,
 'Trampoline': 12,
 'Road / Highway': 13,
 'Under Construction / In Progress Status': 14,
 'Power Lines & Cables': 15,
 'Bridge': 16,
 'Water Tank / Oil Tank': 17,
 'Parking Area - Commercial': 18,
 'Sports Complex / Arena': 19,
 'Industrial Site': 20,
 'Dense Vegetation / Forest': 21,
 'Water Body': 22,
 'Flooded': 23,
 'Boat': 24,
 'Parking Area': 25}*

- reduced the size from (3x3000x4000) to (3x400x400) to speed up the training process

- augmented images (flipping & adjusting color/ brightness, etc.) to improve the accuracy of the model

## Modelling


## Result
