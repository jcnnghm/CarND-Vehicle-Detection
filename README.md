# Vehicle Detection

Submission Notes
---

To detect cars, I:

* Perform a Histogram of Oriented Gradients (HOG) feature extraction on a labeled training set of images and train a Linear SVM classifier
* Append a histograms of color to my HOG feature vector.
* Normalize my features and randomize a selection for training and testing.
* Implement a sliding-window technique and use my trained classifier to search for vehicles in images.
* Run my pipeline on a video stream and create a heat map of recurring detections frame by frame to reject outliers and follow detected vehicles.
* Estimate a bounding box for vehicles detected.

See `Vehicle Tracking.ipynb` file for a complete overview of the pipeline,
with example images and a more extensive overview.

The `output.mp4` file shows the final detected cars, and the
`debug_output.mp4` file contains the output image, as well as images from
each stage of the pipeline.
