-e {"id":"0d835ce2-8bdd-4a4d-a822-78a81a7d3745","object":"chat.completion","created":1771651960,"model":"deepseek-chat","choices":[{"index":0,"message":{"role":"assistant","content":"# Computer Vision: SKILL.md

## Metadata
```yaml
skill_name: Computer Vision
category: Artificial Intelligence
subcategory: Computer Vision & Image Processing
prerequisites:
  - Python programming
  - Linear algebra
  - Calculus
  - Probability & statistics
  - Basic machine learning
difficulty: Intermediate to Advanced
time_to_proficiency: 6-12 months
version: 1.0
last_updated: 2023-11-15
```

## Overview
Computer Vision (CV) is a field of artificial intelligence that enables computers to interpret and understand visual information from the world. It combines techniques from image processing, pattern recognition, and machine learning to extract meaningful information from images and videos.

## Core Concepts

### 1. **Image Fundamentals**
- **Digital Image Representation**: Pixels, color spaces (RGB, HSV, LAB), image formats
- **Image Processing Operations**: Filtering, convolution, edge detection, morphological operations
- **Image Transformations**: Geometric transformations, affine transformations, perspective transforms

### 2. **Feature Detection & Description**
- **Classical Methods**:
  - Harris Corner Detection
  - SIFT (Scale-Invariant Feature Transform)
  - SURF (Speeded-Up Robust Features)
  - ORB (Oriented FAST and Rotated BRIEF)
- **Feature Matching**: Brute-force matching, FLANN, RANSAC for outlier rejection

### 3. **Image Segmentation**
- **Thresholding**: Global, adaptive, Otsu's method
- **Region-based**: Region growing, watershed algorithm
- **Edge-based**: Canny edge detection, active contours
- **Clustering-based**: K-means, mean-shift, DBSCAN
- **Deep Learning-based**: U-Net, Mask R-CNN, DeepLab

### 4. **Object Detection**
- **Traditional Methods**: Viola-Jones, HOG (Histogram of Oriented Gradients) + SVM
- **Deep Learning Approaches**:
  - Two-stage detectors: R-CNN, Fast R-CNN, Faster R-CNN, Mask R-CNN
  - One-stage detectors: YOLO series, SSD (Single Shot MultiBox Detector), RetinaNet
  - Transformer-based: DETR, Vision Transformers

### 5. **Image Classification**
- **Traditional Methods**: Bag of Visual Words, Fisher Vectors
-"},"logprobs":null,"finish_reason":"length"}],"usage":{"prompt_tokens":19,"completion_tokens":500,"total_tokens":519,"prompt_tokens_details":{"cached_tokens":0},"prompt_cache_hit_tokens":0,"prompt_cache_miss_tokens":19},"system_fingerprint":"fp_eaab8d114b_prod0820_fp8_kvcache"}
