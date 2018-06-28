Dissertation for Stephen Bailey
===============================

This is the GitHub repo for Stephen Bailey's dissertation, entitled: *Attributes of Functional Network Architecture Supporting Skilled Reading*. It is currently under construction, and no parts written by me should be considered complete or trustworthy :). It should be complete around August 2018. 



About the Template
==================
This project uses Vanderbilt University's LaTeX template for writing a dissertation. The original GitHub repo for the template can be found at: https://github.com/hootener/LaTeX-Vanderbilt-Dissertation-Format.

Masks are binary arrays which indicate whether a value should be included in an analysis. Masks are the main method for removing or extracting certain parts of an image. Generally,  they are created by applying one or more logical operations to an image. These operations can include:

* Comparisons (e.g., `im > 0`)
* Equality and inequality (`im == 1`, `im ~= 1`)
* Intersections (`(im > 0) & (im < 5)`)
* Unions (`(im < 5) | (im > 10)`)

For this exercise, let's see how well simple thresholds can differentiate between the foreground / background, aTTnd skin / bone.  

*We have imported `plt` for you, and loaded the equalized x-ray image as `im`.*

Create a "foreground" mask by thresholding the image at a value of 50.
Create skin and bone masks by taking foreground pixels with intensities less than 140 (skin) and more than 140 (bone).
Plot the skin and bone masks.