# VCHECK Project
This project aims to provide an automatic process for segmenting the cornea and analyzing the percentage of the specific parts that clinical personnel are concerned about within the entire cornea.


## First Steps: Using SAM to Segment the Cornea
The Segment Anything Model (SAM) is a cutting-edge AI tool developed by Meta AI, designed to "cut out" any object in any image with just a single click. For those interested in learning more, you can read the original paper [here](https://arxiv.org/pdf/2304.02643) and explore the [code](https://github.com/facebookresearch/segment-anything).
They also provide a [demo](https://segment-anything.com/demo) and you could use this demo to segment the cornea.


## Segmenting Clinically Relevant Parts of the Cornea
In this step, we utilize traditional computer vision techniques (OpenCV) to segment the parts of the cornea that are of clinical interest.


The main idea is to use the watershed algorithm to segment the desired portion within the cornea, calculate the minimum enclosing circle based on the corneal contour, and use the center and radius of this circle to compute the percentage of the cornea occupied by the segmented part at different ratio.


We provide a tutorial about our algorithm. Please refer to the "Segment_VCHECK.ipynb" notebook to learn more about our algorithm.
