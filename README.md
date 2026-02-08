# Computer Vision & Augmented Reality Research (2013-2014)

**Undergraduate Research | Osmania University**

This repository contains two research publications from my Bachelor's degree in Electronics and Communication Engineering, focused on feature detection algorithms and camera pose estimation for augmented reality.

---

## Research Publications

### **1. Feature Extraction and Matching using BRISK (2013)**
**Summer Industrial Attachment Programme | May-July 2013**

Implementation and analysis of the Binary Robust Invariant Scalable Keypoints (BRISK) algorithm for efficient feature detection, extraction, and matching.

**Key Contributions:**
- Implemented BRISK feature detection using FAST corner detector
- Developed feature extraction pipeline with scale-space pyramid
- Implemented Hamming distance-based matching for binary descriptors
- Achieved faster computational performance compared to SIFT/SURF while maintaining comparable accuracy

**Technologies:** C++, OpenCV 2.4.3, Microsoft Visual Studio

[📄 Read Full Report](https://github.com/mounicasirineni/computer-vision-ar-research-2013-2014/blob/main/Feature%20Extraction%20and%20Matching%20using%20BRISK.pdf)

---

### **2. Camera Pose Estimation for Augmented Reality Systems (2014)**
**Bachelor's Thesis | 2013-2014**

Real-time camera pose estimation system for augmented reality using monocular SLAM (Simultaneous Localization and Mapping).

**Key Contributions:**
- Developed 6-DOF camera tracking system without prior scene knowledge
- Implemented monocular SLAM using Extended Kalman Filter for state estimation
- Integrated inverse depth parameterization for feature initialization
- Applied 1-Point RANSAC for outlier rejection
- Used quaternions for rotation representation
- Reconstructed 3D camera trajectory from real-time video

**Technologies:** C++, MATLAB, OpenCV, Microsoft Visual Studio

[📄 Read Full Thesis](https://github.com/mounicasirineni/computer-vision-ar-research-2013-2014/blob/main/Camera%20pose%20estimation%20for%20augmented%20reality%20systems.pdf)

---

## Technical Overview

### **Problem Statement**
Augmented reality systems require accurate real-time camera pose estimation to overlay virtual objects onto the physical world. The challenge is achieving this without prior scene knowledge while meeting real-time computational constraints.

### **Approach**

#### **Phase 1: Feature Detection & Matching (BRISK)**
1. **Detection:** FAST algorithm identifies interest points across scale-space pyramid
2. **Extraction:** BRISK descriptor creates binary strings from circular sampling pattern
3. **Matching:** Hamming distance metric efficiently matches binary descriptors between frames

#### **Phase 2: Camera Pose Estimation (SLAM)**
1. **Map Management:** Probabilistic 3D feature map with dynamic addition/deletion
2. **Motion Estimation:** Extended Kalman Filter tracks camera position, orientation, velocity, and angular velocity
3. **Feature Initialization:** Inverse depth parameterization handles features from near to infinity
4. **Outlier Rejection:** 1-Point RANSAC filters spurious matches using EKF predictions
5. **Pose Recovery:** Quaternion-based rotation with 6-DOF camera trajectory reconstruction

---

## Key Algorithms

### **Feature Detection & Description**
- FAST (Features from Accelerated Segment Test)
- BRISK (Binary Robust Invariant Scalable Keypoints)
- Scale-space pyramid construction
- Hamming distance matching

### **SLAM Components**
- Extended Kalman Filter (EKF)
- Inverse depth parameterization
- Quaternion-based rotation
- 1-Point RANSAC
- Gaussian smoothing

---

## Results

### **BRISK Feature Detection**
- Frame 1: 198 keypoints detected
- Frame 2: 187 keypoints detected
- Successfully matched features across consecutive video frames
- Faster performance than SIFT/SURF with comparable accuracy

### **SLAM Trajectory Estimation**
- Built probabilistic 3D maps in unknown environments
- Achieved drift-free localization over repeated movements
- Real-time processing on monocular camera
- Robust handling of high-acceleration motion

---

## Background

This research was conducted during my Bachelor's degree in Electronics and Communication Engineering at Osmania University (2010-2014).

Through a university collaboration with **Thinc Innovations**, a computer vision startup in Hyderabad, I had the opportunity to work on practical CV applications under the guidance of **Mr. P. Balakrishna Reddy**, who was building their Computer Vision division.

**Summer 2013:** Industrial attachment focused on feature detection algorithms (BRISK implementation)

**2013-2014:** Undergraduate thesis extending this work to camera pose estimation for augmented reality using monocular SLAM and Extended Kalman Filters

---

## Technical Stack

**Languages:** C++, MATLAB

**Libraries:** OpenCV 2.4.3, MATLAB Computer Vision Toolbox

**Tools:** Microsoft Visual Studio

**Algorithms:** FAST, BRISK, Extended Kalman Filter, RANSAC, Inverse Depth Parameterization, Quaternions

---

## Publications

**[1]** S. Mounica, V.S.V. Rama Madhuri, S. Sneha, "Feature Extraction and Matching using BRISK," Mini Project Report, Department of Electronics and Communication Engineering, University College of Engineering, Osmania University, July 2013.

**[2]** S. Mounica, V.S.V. Rama Madhuri, S. Sneha, "Camera Pose Estimation for Augmented Reality Systems," Bachelor of Engineering Thesis, Department of Electronics and Communication Engineering, University College of Engineering, Osmania University, May 2014.

---

## Acknowledgments

**Research Advisor:**
- Mr. P. Balakrishna Reddy, Computer Vision Architect, Thinc Innovations

**Faculty Advisors:**
- Dr. P. Ananth Raj, Professor, Department of ECE, Osmania University
- Dr. P. Chandra Sekhar, Head of Department, ECE, Osmania University

**Team Members:**
- S. Mounica
- V.S.V. Rama Madhuri  
- S. Sneha

---

## References

1. Stefan Leutenegger, Margarita Chli, Roland Y. Siegwart, "BRISK: Binary Robust Invariant Scalable Keypoints," Autonomous Systems Lab, ETH Zürich
2. A. J. Davison et al., "MonoSLAM: Real-time Single Camera SLAM," IEEE TPAMI, 2007
3. E. Rosten, T. Drummond, "FASTER and Better: A Machine Learning Approach to Corner Detection," IEEE TPAMI, 2010

---

## License

This research was conducted as part of undergraduate academic work at Osmania University. The publications are shared for educational and reference purposes.

---

## Contact

**S. Mounica**  
LinkedIn: www.linkedin.com/in/mounicasirineni
Email: mounicasirineni@gmail.com

---

**Last Updated:** February 2026
