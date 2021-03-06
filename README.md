# focal-tversky-unet

Code accompanying our paper [A novel focal Tversky loss function and improved Attention U-Net for lesion segmentation](https://arxiv.org/abs/1810.07842) accepted at [ISBI 2019](https://biomedicalimaging.org/2019/).

If you find this code useful, please consider citing our work:

```
@article{focal-unet,
  title={A Novel Focal Tversky loss function with improved Attention U-Net for lesion segmentation},
  author={Abraham, Nabila and Khan, Naimul Mefraz},
  journal={arXiv preprint arXiv:1810.07842},
  year={2018}
}
```

Training files for the ISIC2018 and BUS2017 Dataset B have been added. 
If training with ISIC2018, create 4 folders: `orig_raw` (not used in this code), `orig_gt`, `resized-train`, `resized-gt`, for full 
resolution input images, ground truth and resized images at `192x256` resolution.

If training with BUS2017, create 2 folders: `original` and `gt` for input data and ground truth data. In the `bus_train.py` script, images 
will be resampled to `128x128` resolution. 
