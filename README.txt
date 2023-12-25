Project Description:
This project is centered around advanced image processing techniques, focusing on feature detection, descriptor extraction, and feature matching using various algorithms. The goal is to explore different methods for detecting interest points, extracting feature descriptors, and matching these features across different images or the same image under varying conditions.

Program Structure:
1. Harris Corner Detection:
The program uses the Harris Corner Detector to identify interest points in the image.
The detected corners are highlighted and visualized.
2. Shi-Tomasi Corner Detector:
Implements the Shi-Tomasi Corner Detector to find keypoints in the image.
Extracts patches around each keypoint for further processing.
3. SIFT Feature Detection and Matching:
Utilizes the SIFT (Scale-Invariant Feature Transform) algorithm to detect and compute feature descriptors.
Performs feature matching based on the descriptors using Normalized Cross Correlation (NCC) and L2 distance measures.
Visualizes the top matches obtained by each method.
4. Harris Corner-Based Feature Description and Matching:
After detecting corners with the Harris Corner Detector, the program extracts feature descriptors around these points.
Matches these features using Normalized Cross Correlation (NCC) and displays the results.

Implementation Details:
Harris Corner Detection: Utilizes OpenCV's cornerHarris function.
Shi-Tomasi Corner Detector: Employs goodFeaturesToTrack for keypoint detection.
SIFT Features: Uses OpenCV's SIFT_create for feature detection and descriptor computation.
Feature Matching: Implemented using both NCC and L2 distance metrics.
Normalized Cross Correlation (NCC): Custom implementation for matching descriptors.
Visualization: Matplotlib is used for displaying images and feature matches.

Usage:
Ensure that the required Python libraries (opencv-python, numpy, matplotlib) are installed.
Replace the image paths with your local image file paths.
Run each script to see the feature detection and matching results for different algorithms.

Output:
The output of the project includes visualizations of detected features and their matches across images, showcasing the effectiveness of each technique used.