# SIFT_vs_ORB_vs_FAST_and_ORB
A Jupyter Notebook comparing keypoint detection and matching algorithms (SIFT, ORB, FAST+ORB) on images with BFMatcher and RANSAC filtering.

###  Environment setup

If you are working in Google Colab, install the dependencies:

``` bash
!pip install opencv-python opencv-contrib-python matplotlib
```
###  Algorithms used

-   **SIFT (Scale-Invariant Feature Transform)** --- robust to scale and
    rotation changes.\
-   **ORB (Oriented FAST and Rotated BRIEF)** --- fast and lightweight,
    suitable for real-time applications.\
-   **FAST + ORB** --- FAST detector combined with ORB descriptor.

###  Main steps of the notebook

1.  Load the image `miem.jpg` and resize it.\
2.  Apply an affine transformation to distort the image.\
3.  Detect keypoints using SIFT, ORB, and FAST+ORB.\
4.  Match keypoints between original and transformed images using
    BFMatcher.\
5.  Apply RANSAC to filter out false matches and estimate the
    transformation.\
6.  Display metrics and matched images.\
7.  Plot a comparative bar chart of the algorithms.

###  Conclusions

-   **SIFT** provides high-quality matches but is slower.\
-   **ORB** is fast and lightweight but may produce fewer matches.\
-   **FAST + ORB** combines the speed of FAST with the robustness of
    ORB.

