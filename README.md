# MRI_DICOM_data_reading_visualization
This project aims to read and visualise DICOM, mha or nrrd images from a directory containing many patients using simpleitk library and python

# Requirements : 

-Python 3.5.2

-SimpleITK

-matplotlib.pyplot

# imports :
import os

import sys

import warnings

import SimpleITK as sitk

from skimage.transform import resize

from skimage.morphology import label

from skimage.io import imread, imshow, imread_collection, concatenate_images

import numpy as np

from skimage import io

import matplotlib.pyplot as plt

%matplotlib inline

# Data :

The data shoulde be stuctred in drectory like this :

Main_Data_Folder/

--> Patitent1

  -->MRI1.dcm (or .mha, .nrrd ...)

  -->MRI2.dcm ((or .mha, .nrrd ...)

--> patiant2

  -->MRI1.dcm (or .mha, .nrrd ...)

  -->MRI2.dcm ((or .mha, .nrrd ...)

.

.

.

--> patiantN

  -->MRI1.dcm (or .mha, .nrrd ...)

  -->MRI2.dcm ((or .mha, .nrrd ...)

So, I think that i think that you got what I mean, for every patient, the Dicom files should be named similarly  
