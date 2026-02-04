# Computer Vision & Augmented Reality Research (2013-2014)
# Undergraduate Research in SLAM, Feature Detection, and AR Systems
This repository contains my undergraduate research work in computer vision and augmented reality conducted at Osmania University (2013-2014) under the guidance of Mr. P. Balakrishna Reddy (Computer Vision Architect, Thinc Innovations).
# Research Publications
1. Feature Extraction and Matching using BRISK (2013)
   
Summer Industrial Attachment Programme | May-July 2013

Implementation and analysis of the Binary Robust Invariant Scalable Keypoints (BRISK) algorithm for efficient feature detection, extraction, and matching in computer vision applications.

Key Contributions:
- Implemented BRISK feature detection using FAST (Features from Accelerated Segment Test) corner detector
- Developed feature extraction pipeline with scale-space pyramid for rotation and scale invariance
- Implemented Hamming distance-based feature matching for binary descriptors
- Achieved dramatically faster computational performance compared to SIFT/SURF while maintaining comparable matching accuracy

Technologies: 
C++, OpenCV, Microsoft Visual Studio

2. Camera Pose Estimation for Augmented Reality Systems (2014)

Bachelor's Thesis | 2013-2014

Complete implementation of a real-time camera pose estimation system for augmented reality applications using monocular SLAM (Simultaneous Localization and Mapping) combined with computer vision techniques.

Key Contributions:
- Developed 6-DOF (six degrees of freedom) camera tracking system without prior scene knowledge
- Implemented monocular SLAM using Extended Kalman Filter (EKF) for probabilistic state estimation
- Integrated inverse depth parameterization for efficient feature initialization at varying distances
- Applied 1-Point RANSAC algorithm for robust outlier rejection in feature matching
- Used quaternions for rotation representation and camera motion modeling
- Successfully reconstructed 3D camera trajectory from real-time video sequences

Technologies: C++, MATLAB, OpenCV, Microsoft Visual Studio

# Technical Overview

Problem Statement

Augmented reality systems require accurate real-time camera pose estimation to overlay virtual objects onto the physical world. Traditional methods either require prior knowledge of the scene or fail to handle the computational constraints of real-time processing.

Approach

Phase 1: Feature Detection & Matching (BRISK)
1. Detection: FAST algorithm identifies interest points across scale-space pyramid
2. Extraction: BRISK descriptor creates binary strings from circular sampling pattern
3. Matching: Hamming distance metric efficiently matches binary descriptors between frames

Phase 2: Camera Pose Estimation (SLAM)
1. Map Management: Probabilistic 3D feature map with dynamic addition/deletion
2. Motion Estimation: Extended Kalman Filter tracks camera position, orientation, velocity, and angular velocity
3. Feature Initialization: Inverse depth parameterization handles features from near to infinity
4. Outlier Rejection: 1-Point RANSAC filters spurious matches using EKF predictions
5. Pose Recovery: Quaternion-based rotation with 6-DOF camera trajectory reconstruction

# Key Algorithms Implemented
Feature Detection & Description
- FAST (Features from Accelerated Segment Test): Corner detection in scale-space
- BRISK (Binary Robust Invariant Scalable Keypoints): Binary descriptor generation
- Scale-Space Pyramid: Octaves and intra-octaves for scale invariance
- Hamming Distance: Efficient binary descriptor matching

SLAM Components
- Extended Kalman Filter (EKF): Probabilistic state estimation and prediction
- Inverse Depth Parameterization: Unified representation for near and distant features
- Quaternions: Efficient 3D rotation representation
- 1-Point RANSAC: Outlier rejection using minimal feature correspondences
- Gaussian Smoothing: Noise reduction in intensity sampling

# Results
BRISK Feature Detection
- Frame 1: 198 keypoints detected
- Frame 2: 187 keypoints detected
- Matched Features: Successfully matched across consecutive video frames
- Performance: Dramatically faster than SIFT/SURF with comparable accuracy

SLAM Trajectory Estimation
- Successfully built probabilistic 3D maps in unknown environments
- Achieved drift-free localization over repeated camera movements
- Real-time processing on single monocular camera
- Robust handling of high-acceleration motion

# Publications
[1] S. Mounica, V.S.V. Rama Madhuri, S. Sneha, "Feature Extraction and Matching using BRISK," Mini Project Report, Department of Electronics and Communication Engineering, University College of Engineering, Osmania University, July 2013.

[2] S. Mounica, V.S.V. Rama Madhuri, S. Sneha, "Camera Pose Estimation for Augmented Reality Systems," Bachelor of Engineering Thesis, Department of Electronics and Communication Engineering, University College of Engineering, Osmania University, May 2014.

# Acknowledgments
Advisors:
- Mr. P. Balakrishna Reddy, Computer Vision Architect, Thinc Innovations
- Dr. P. Ananth Raj, Former Professor, Department of ECE, Osmania University
- Dr. P. Chandra Sekhar, Head of Department, ECE, Osmania University

Team:
- S. Mounica
- V.S.V. Rama Madhuri
- S. Sneha

# References
Key Papers:
1. Stefan Leutenegger, Margarita Chli, Roland Y. Siegwart, "BRISK: Binary Robust Invariant Scalable Keypoints," Autonomous Systems Lab, ETH Zürich
2. A. J. Davison et al., "MonoSLAM: Real-time Single Camera SLAM," IEEE TPAMI, 2007
3. E. Rosten, T. Drummond, "FASTER and Better: A Machine Learning Approach to Corner Detection," IEEE TPAMI, 2010

# License
This research was conducted as part of undergraduate academic work at Osmania University. The publications are shared for educational and reference purposes.
