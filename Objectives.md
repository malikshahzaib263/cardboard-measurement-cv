# Measurable Objectives

## MO-1 — Physical Measurement Accuracy

Measured quantity:
Absolute width and height error in millimetres.

Method:
Compare model measurements against ruler or calliper
measurements for at least 10 instances.

Target:
Not established before testing.

Result:
Not measured.

Status:
Incomplete. No valid real-camera calibration or
pixel-to-millimetre reference was available.

## MO-2 — Segmentation Performance

Measured quantity:
Mean Dice score on the held-out test set.

Method:
Compare thresholded U-Net predictions with the
available SAM-derived reference masks.

Threshold:
0.50

Test images:
7

Observed Dice:
0.6099

Observed IoU:
0.5243

Observed Precision:
0.5683

Observed Recall:
0.7371

Note:
These are observed results, not evidence that a
performance target was set before training.

## Additional Results

Pixel-level mean AP: 0.6479

Connected-component AP@0.50 approximation: 0.4881

Connected-component AP@0.50:0.95 approximation: 0.3500

These AP measurements use different evaluation
definitions and should not be treated as interchangeable.

## Limitations
- Small test set.
- SAM-generated labels not fully manually verified.
- Weak predictions on cardboard_070.jpg and
  cardboard_075.jpg.
- Random image split may include views of the
  same physical object in different subsets.
- No verified physical dimension accuracy.
