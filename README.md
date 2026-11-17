# Cardboard Segmentation — Measure It Assessment

## Project Status
Partial implementation.

## Dataset
- Original photographs: 78
- Generated SAM masks: 76
- Retained image-mask pairs: 68
- Training: 47
- Validation: 14
- Testing: 7

## Model
U-Net semantic segmentation model.

Input resolution: 256 x 256 pixels.

Saved model:
cardboard_unet_clean.keras

SHA-256:
d82e37b4f07104fe413b797edf950f2c5a3a15ac35083d70a0a5f97a4d567cbe

## Evaluation
Test Dice: 0.6099

Test IoU: 0.5243

Test Precision: 0.5683

Test Recall: 0.7371

Pixel AP: 0.6479

Approximate connected-component AP@0.50: 0.4881

Approximate connected-component AP@0.50:0.95: 0.3500

## Available Artifacts
- test_metrics.csv
- pixel_average_precision.csv
- instance_ap_approximation.csv
- split_manifest.json
- project_status.json
- synthetic_calibration_practice.npz

## Camera Calibration
The calibration experiment used synthetic
checkerboard images.

RMS reprojection error: approximately 6.2619 pixels.

This does not establish calibration of the actual
camera used to photograph the cardboard.

## Not Implemented
- Valid image-to-millimetres measurement
- Physical width and height error evaluation
- Real-camera undistortion comparison
- Validated measurement confidence handling

## Reproducibility
Original notebooks, dataset, saved model and
dependencies must be included or linked.

The current split manifest was exported after
training and is not proof of a pre-training commit.

Hardware, software versions, camera model and
full execution instructions remain to be documented.

## Project Files — Google Drive

The project was developed and trained using Google Colab.

### Training Notebook
[Open Cardboard Segmentation Notebook](PASTE_NOTEBOOK_GOOGLE_DRIVE_LINK_HERE)

### Trained U-Net Model
[Download Trained U-Net Model](PASTE_MODEL_GOOGLE_DRIVE_LINK_HERE)

**Model:** U-Net  
**Model file:** `cardboard_unet_clean.keras`

**SHA-256:** `d82e37b4f07104fe413b797edf950f2c5a3a15ac35083d70a0a5f97a4d567cbe`

### Evaluation Results
- Test Dice: 0.6099
- Test IoU: 0.5243
- Precision: 0.5683
- Recall: 0.7371
- Pixel Average Precision: 0.6479

### Limitations
Real-camera calibration, reliable millimetre measurement and physical accuracy validation remain incomplete. Synthetic checkerboard calibration was performed for practice only.
