# dual-contrastive-learning

* [Datasets](https://drive.google.com/drive/folders/1BfTWjdWP05WcjJUVEtTaHN1HN-G4Xy9w?usp=sharing) (A domain (unstained images) to B domain (stained images))

## Fréchet inception distance (FID) calculation
We used an already implemented FID calculator that uses PyTorch. Repository can be reviewed via visiting [here](https://github.com/mseitzer/pytorch-fid/tree/master).
### How to use ?
README section of the repository is pretty clear yet, we're including the necessary commands here also. (If you encounter any error, check the issues section of the repository.)

Installation using pip:
```
pip install pytorch-fid
pip install --user scipy==1.11.1
```
(Installing 1.11.1 version of scipy is necessary if your current version is >= 1.11.2)

To compute the FID score between two datasets, where images of each dataset are contained in an individual folder:
```
python -m pytorch_fid path/to/dataset1 path/to/dataset2
```


## Kernel inception distance (KID) calculation

Installation using pip:
```
pip install torchmetrics
pip install pillow
```

You can go to the KidCalculation.ipynb file and run the cell with the desired image paths.


## Structural similarity index measure (SSIM) calculation

Installation using pip:
```
pip install pillow
```

You can go to the SSIM Calculation.ipynb file and run the cell with the desired image paths.
