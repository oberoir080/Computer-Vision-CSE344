# Computer Vision Assignments

This repository contains a comprehensive collection of Computer Vision assignments covering fundamental concepts, advanced techniques, and practical implementations. Each assignment focuses on different aspects of computer vision, from basic image processing to advanced deep learning models.

> **Note:** These assignments were completed as part of the coursework for Computer Vision (CSE344) at IIIT Delhi, taught by Dr. Saket Anand in the Winter 2025 semester.

## Assignment Overview

### HW1: Fundamentals of Computer Vision

#### Classification
- **Objective**: Image classification using traditional computer vision techniques
- **Outputs**: 
  - Classification results on various image datasets
  - Performance metrics and accuracy scores
  - Visualization of classification boundaries

#### Tracking
- **Objective**: Object tracking in video sequences using MOT17 dataset
- **Outputs**:
  - Frame analysis from MOT17-11-SDP and MOT17-13-SDP sequences
  - Data distribution analysis showing frame counts across sequences
  - Visualization of tracking sequences and frame statistics
- **Inferences**: 
  - Different sequences have varying frame counts, affecting tracking complexity
  - MOT17-11-SDP and MOT17-13-SDP provide diverse tracking scenarios

---

### HW2: Camera Calibration and 3D Vision

#### Camera Calibration (Q3)
- **Objective**: Calibrate camera using chessboard patterns
- **Outputs**:
  - **Intrinsic Camera Matrix**: Complete camera calibration parameters
  - **Focal Lengths**: fx and fy values for camera optics
  - **Skew Parameter**: Camera sensor alignment information
  - **Principal Point**: Optical center coordinates (cx, cy)
  - **Radial Distortion Coefficients**: k1, k2, k5 for lens distortion correction
  - **Rotation Matrices**: 3D orientation for each calibration image
  - **Translation Vectors**: 3D position for each calibration image
- **Inferences**:
  - Camera calibration accuracy depends on chessboard corner detection
  - Distortion correction significantly improves image quality
  - Multiple calibration images provide robust parameter estimation

#### Panorama Stitching (Q4)
- **Objective**: Create panoramic images from multiple overlapping photos
- **Outputs**:
  - **Image Clustering**: K-means clustering of panorama dataset (k=3)
  - **SIFT Feature Detection**: Keypoint extraction and matching
  - **Homography Verification**: Geometric transformation validation
  - **Feature Matching**: BF and FLANN matcher comparisons
- **Inferences**:
  - Histogram-based clustering groups similar images effectively
  - SIFT features provide robust matching across different viewpoints
  - Homography verification ensures geometric consistency

#### Point Cloud Registration (Q5)
- **Objective**: Align 3D point clouds using ICP algorithm
- **Outputs**:
  - **Transformation Matrices**: 4x4 rigid body transformations
  - **Registration Quality Metrics**: Fitness scores and RMSE values
  - **Hyperparameter Optimization**: Best threshold, iterations, and initialization
- **Inferences**:
  - RANSAC-based initialization provides better convergence than random
  - Optimal threshold values depend on point cloud density
  - FPFH features improve initial alignment for complex geometries

---

### HW3: Advanced Computer Vision with Deep Learning

#### CLIP Text-Image Scoring (Q1)
- **Objective**: Evaluate text-image similarity using CLIP and CLIPS models
- **Outputs**:
  - **Similarity Scores**: Quantitative measures of text-image alignment
  - **Model Comparison**: CLIP vs CLIPS performance analysis
  - **Text Descriptions**: 10 diverse text prompts for evaluation
- **Inferences**:
  - CLIP provides robust text-image similarity assessment
  - CLIPS shows improved performance on specific domains
  - Semantic understanding varies with text complexity

#### Visual Question Answering (Q2)
- **Objective**: Answer questions about images using BLIP model
- **Outputs**:
  - **Question-Answer Pairs**: Spatial and descriptive queries
  - **Model Responses**: Natural language answers to visual questions
  - **Spatial Understanding**: Location-based question answering
- **Inferences**:
  - BLIP demonstrates strong spatial reasoning capabilities
  - Model can identify object locations and relationships
  - VQA performance depends on question complexity and image content

#### Image Captioning and Evaluation (Q3)
- **Objective**: Generate captions and evaluate them using multiple models
- **Outputs**:
  - **BLIP Captions**: Natural language descriptions of images
  - **CLIP Scores**: Caption-image alignment metrics
  - **CLIPS Scores**: Alternative similarity measurements
- **Inferences**:
  - BLIP generates contextually relevant captions
  - CLIP scores correlate with caption quality
  - Multiple evaluation metrics provide comprehensive assessment

#### Referring Expression Segmentation (Q4)
- **Objective**: Segment objects based on natural language descriptions
- **Outputs**:
  - **Segmentation Masks**: Pixel-level object segmentation
  - **Overlay Visualizations**: Original images with segmentation overlays
  - **Text-Image Alignment**: Precise object localization from text
- **Inferences**:
  - Model can handle complex referring expressions
  - Segmentation quality depends on text description clarity
  - BERT tokenization improves text understanding

#### SAM-based Segmentation with DINOv2 (Q5)
- **Objective**: Advanced segmentation using Segment Anything Model and DINOv2
- **Outputs**:
  - **Automatic Mask Generation**: SAM-based segmentation
  - **Feature Matching**: DINOv2-based image similarity
  - **Mask Processing**: Refined segmentation boundaries
- **Inferences**:
  - SAM provides high-quality initial segmentation
  - DINOv2 features enable robust image matching
  - Combined approach improves segmentation accuracy

