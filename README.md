# Clothing Pattern Dataset
A large dataset containing images of clothing patterns across six classes: solid, striped, dotted, checkered, zigzag, and floral.

Note that the images in this dataset may be subject to copyright, and so we do not make them publicly available. Instead, we provide URLs to download the original images, along with cropping/scaling information needed to reconstruct the dataset.

Refer to the file googleClothingDataset.csv to download the dataset images. Each line contains a single image source, with the class name, image URL, original dimensions, crop window, and one or more scales. For each downloaded image, first crop the image using the provided rectangle and then create synthetic variations as follows:
* Generate 224x224 pixel images with the cropped original image centered in the frame.
* Use the values listed to scale the image
* For each scale, generate 12 variations by rotating the image in 30 degree increments

The images included in the FingerCamera folder are free to use without restriction. If you publish any works using these images, please cite the following paper:

```
@InProceedings{medeirosClothingColorsAndVisualTextures,
	      Author    = {Alexander J. Medeiros and Lee Stearns and Leah Findlater and Chuan Chen and Jon E. Froehlich},
	      Title     = {Recognizing Clothing Colors and Visual Textures Using a Finger-Mounted Camera: An Initial Investigation},
	      Booktitle = {Proceedings of the 19th International ACM SIGACCESS Conference on Computers and Accessibility  - ASSETS '17},
	      Year      = {2017}}
```
