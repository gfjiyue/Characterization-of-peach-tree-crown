# Characterization of peach tree crown by using high-resolution images from an unmanned aerial vehicle

**This is a support page of paper published at "Horticulture Research" as an Original Research.**
> Yue Mu, Yuichiro Fujii, Daisuke Takata, Bangyou Zheng, Koji Noshita, Kiyoshi Honda, Seishi Ninomiya, Wei Guo*. Characterization of peach tree crown by using high-resolution images from an unmanned aerial vehicle, Horticulture Research, 2018.

Article DOI: 10.1038/s41438-018-0097-z

## 1 Data
### a. Raw UAV images
Images for peach trees can be collected by DJI inspire 1 (Shenzhen Dajiang Baiwang Technology Co., Ltd, China), controlled by Litchi software (VC Technology Ltd, UK) to direct it flying along a double-grid image acquisition plan, at a height of 30 m and a speed of 2.5 m/s with the camera looking downwards.

**Make sure the overlap of photos to the front and side is high enough to generate dense point cloud.**

![](https://github.com/UTokyo-FieldPhenomics-Lab/Efficient-characterization-of-peach-tree-crown-/blob/master/figure/FIG21.jpg) 
The numbers label the flight order of way point and the red points mark the ground control points.

### b. Digital surface model (DSM)
DSM can be generated in Pix4Dmapper Pro v. 4.0.25 software (Pix4D Inc., Switzerland) by using the raw images. 

During the matching of photos, full image scale was set for precisely extracting the key points and the relative camera positions were also taken into account to discard geometrically unrealistic matches. In addition, **use the coodinates of ground control points to optimize the georeferencing of the point cloud**. During the generation of DSM, noise filtering was used to correct the altitude of these points with the median altitude of the neighbouring points. 


## 2 Processing 
### Step 1. Download source codes from the link below, and put them in one folder.

**To download the example data and codes, please fill a simple form below:**

https://goo.gl/forms/e0HaPDcKfK4OQVTW2

The download link will be sent to your email once the form is completed.

### Step 2. Generate the branch map by using bare-branch DSM in winter
Edit the file path and parameters, then run Branch_map.m

### Step 3. Calculate the crown characters by using the foliated DSM in summer
Edit the file path and parameters, then run Crown_map.m

## 3 Results
### a. Crown map (tif)
### b. Crown parameters (excel)

