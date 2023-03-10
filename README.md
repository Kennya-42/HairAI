# HairAi
Fork from https://github.com/ZPdesu/Barbershop.git

Goal:
Create Gui front end to create user friendly use. Allow users to use AI to see themselves with potential hair styles free of charge.

## Installation
- Clone the repository:
``` 
git clone https://github.com/Kennya-42/HairAI.git
cd HairAi
```
- Dependencies:  
We recommend running this repository using [Anaconda](https://docs.anaconda.com/anaconda/install/). 
All dependencies for defining the environment are provided in `environment/environment.yaml`.


## Download II2S images
Please download the [II2S](https://drive.google.com/drive/folders/15jsR9yy_pfDHiS9aE3HcYDgwtBbAneId?usp=sharing) 
and put them in the `input/face` folder.


## Getting Started  
Preprocess your own images. Please put the raw images in the `unprocessed` folder.
```
python align_face.py
```

Produce realistic results:
```
python main.py --im_path1 90.png --im_path2 15.png --im_path3 117.png --sign realistic --smooth 5
```

Produce results faithful to the masks:
```
python main.py --im_path1 90.png --im_path2 15.png --im_path3 117.png --sign fidelity --smooth 5
```