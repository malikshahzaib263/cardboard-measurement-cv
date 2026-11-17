# Project Plan — Measure It

## Objective
Develop a computer vision pipeline to segment cardboard
and estimate real-world width and height in millimetres.

## Intended Workflow
1. Calibrate the camera with checkerboard images.
2. Collect and label cardboard photographs.
3. Train a segmentation model.
4. Evaluate segmentation performance.
5. Convert image pixels to millimetres.
6. Compare measurements against physical ground truth.

## Work Actually Completed
- 78 real cardboard photographs collected.
- 76 SAM-generated masks.
- 68 image-mask pairs retained.
- U-Net trained and evaluated.
- Synthetic checkerboard calibration experiment.
- Segmentation metrics and model hash exported.

## Incomplete Work
- Real camera calibration.
- Valid pixel-to-millimetre conversion.
- Physical measurement error evaluation.
- Raw-versus-undistorted measurement comparison.
- Controlled failure-condition experiment.

## Decision Record
U-Net was chosen instead of Ultralytics YOLO or a
Roboflow segmentation model.

SAM was used to generate candidate labels.

Eight masks were excluded based on suspiciously
small foreground coverage. Their correctness was
not fully established through manual review.

Synthetic checkerboard calibration was retained
as a practice experiment, not real-camera evidence.

## Documentation Note
This plan records the work retrospectively.
It must not be represented as a plan committed
before implementation.
