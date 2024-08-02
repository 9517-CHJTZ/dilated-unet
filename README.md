## Download Dataset

Dataset and the Jupyter notebook needs to be structured as:

### Method 1

```
.
+-- dilated-U-net
|   +-- projectcode
    |   +-- unet_dilated.ipynb
|   +-- test.csv
|   +-- train.csv
|   +-- val.csv
+-- 61541v001
|   +-- data
    |   +-- WildScenes
        |   +-- WildScenes2d
```

### Method 2

```
61541v001/
├── data/                   
├── metadata/               
├── projectcode/            
│   ├── Unet_dw_20.ipynb    
│   └── Unet_dw_100.ipynb   
├── test.xlsx               
├── train.xlsx              
└── val.xlsx                
```



## Run method 1 ( U-Net + Dilated Convolution) Code

* System: WSL (If you are using Windows, please comment out the code change path in the `unet_dilated.ipynb`)

* Download anaconda environment

```
conda env create --file environment.yml
conda activate dilated_unet
```

* Go to the directory contains the Jupyter notebook file, and run all cells in `unet_dilated.ipynb` the model will start training



## Run method 2 ( U-Net + Depth-wise Convolution) Code

* System: Windows

* Requirements: 

  Python 3.8 or higher

  PyTorch

  torchvision

  numpy

  matplotlib

  pandas

  Jupyter Notebook

```
pip install torch torchvision numpy matplotlib pandas jupyter
```

* Change the dataset file path on Jupyter notebook file, and run all cells in `Unet_dw_20.ipynb` the model will start training
