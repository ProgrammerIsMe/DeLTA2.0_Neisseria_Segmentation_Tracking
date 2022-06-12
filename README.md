# DeLTA2.

## Background
Our research aims to segment and track bacteria that are growing in two dimensions
Using our own dataset, we train a new model for accurate segmentation

## Steps
1. Preparation for starting: show gpu and memory information
2. Pip install necessary packages: install all the necessary packages
3. Load functions for image display: function to show image frames
4. Generate weight map: use delta.data.seg_weights_2D()
5. Rename the images: load the images in each folder and rename it as s1_1
6. Combine all the images together: combine all the images in img, seg and wei
7. Pre-processing: image normalization and invert to generate the images for network input
8. Train own model: 
- split 10% dataset for validation
- train model and save it as unet_pads_seg.hdf5
- calculate the accuracy on test dataset using tf.keras.metrics.BinaryAccuracy()
9. Display the output images: show the images in sequences step by step
10. Test the model performace: test segmentation network and tracking network together


## Version
DeLTA2_v2.ipynb is the latest version

## Reference
[1] O’Connor, Owen M., et al. "DeLTA 2.0: A deep learning pipeline for quantifying single-cell spatial and temporal dynamics." PLOS Computational Biology 18.1 (2022): e1009797.