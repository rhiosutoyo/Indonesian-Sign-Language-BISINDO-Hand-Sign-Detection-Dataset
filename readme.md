
# Indonesian Sign Language (BISINDO) Hand Sign Detection Dataset

This repository contains datasets related to our paper [BISINDO Hand-Sign Detection Using Transfer Learning](https://doi.org/10.1109/ICRAIE59459.2023.10468194).

## Data Collection: BISINDO Hand Sign
The dataset contains 20 photos for each character (i.e., A-Z). All the images were taken using a smartphone camera (i.e., Redmi Note 10 Pro) and processed using Python OpenCV. 
The same setting parameters are applied to all the photos (e.g., light intensity and distance). The total number of pictures in the dataset is 520 photos.

## Data Labeling
All photos are labeled using a Python package called [labelImg](https://pypi.org/project/labelImg/1.4.0/). 
Each photo has a label in the form of an XML file that contains information, such as the photo’s directory, name, size, label, box coordinates, etc. 
The XML structure is shown below.

```xml
<?xml version="1.0" encoding="utf-8"?>
<annotation>
	<folder>allimages</folder>
	<filename>file-name.jpg</filename>
	<path>folder-path\file-name.jpg</path>
	<source>
		<database>Unknown</database>
	</source>
	<size>
		<width>640</width>
		<height>480</height>
		<depth>3</depth>
	</size>
	<segmented>0</segmented>
	<object>
		<name>A</name>
		<pose>Unspecified</pose>
		<truncated>0</truncated>
		<difficult>0</difficult>
		<bndbox>
			<xmin>186</xmin>
			<ymin>214</ymin>
			<xmax>460</xmax>
			<ymax>344</ymax>
		</bndbox>
	</object>
</annotation>
```

## Data Processing
The images are in the [collected images](https://github.com/rhiosutoyo/Research-Binus-BISINDO-DATASET/tree/master/collectedimages) folder. The dataset is separated into two groups, training, and testing, with a ratio of 4:1.
- [Training](https://github.com/rhiosutoyo/Research-Binus-BISINDO-DATASET/tree/master/train)
- [Testing](https://github.com/rhiosutoyo/Research-Binus-BISINDO-DATASET/tree/master/test)

##  Citation
If you use this dataset in a scientific publication, we would appreciate using the following citations:

### Plain Text
D. Joan, V. Vincent, K. J. Daniel, S. Achmad and R. Sutoyo, "BISINDO Hand-Sign Detection Using Transfer Learning," 2023 IEEE 8th International Conference on Recent Advances and Innovations in Engineering (ICRAIE), Kuala Lumpur, Malaysia, 2023, pp. 1-7, doi: 10.1109/ICRAIE59459.2023.10468194.

### BibTeX
```
@INPROCEEDINGS{10468194,
  author={Joan, David and Vincent, Vincent and Daniel, Kevin Jason and Achmad, Said and Sutoyo, Rhio},
  booktitle={2023 IEEE 8th International Conference on Recent Advances and Innovations in Engineering (ICRAIE)}, 
  title={BISINDO Hand-Sign Detection Using Transfer Learning}, 
  year={2023},
  volume={},
  number={},
  pages={1-7},
  keywords={Sign language;Computer vision;Technological innovation;Computational modeling;Transfer learning;Refining;Assistive technologies;Hand Sign Recognition;Computer Vision;Object Detection;BISINDO;Transfer Learning},
  doi={10.1109/ICRAIE59459.2023.10468194}}
```
