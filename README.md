# Image Restoration and Noise Analysis in Solar Imagery

This Jupyter Notebook presents a comprehensive workflow for analyzing, restoring, and segmenting a degraded solar image composed of multiple noisy quadrants.  
The project is designed as an academic exercise in image processing, focusing on noise identification, restoration filtering, and feature segmentation.

---

## 🧠 Project Overview

The notebook performs the following main tasks:

1. **Image Decomposition**
   - Loads the original and clean solar images.
   - Divides them into four quadrants for localized analysis.

2. **Noise Characterization**
   - Identifies different noise types in each quadrant:
     - Gaussian and Rayleigh noise (Upper Left)
     - Uniform noise with intensity scaling (Upper Right)
     - Salt-and-pepper noise (Lower Left)
     - Additive periodic noise (Lower Right)

3. **Image Restoration**
   - Applies suitable filters for each noise type:
     - Median and Alpha-Trimmed Mean filters  
     - Arithmetic Mean filter  
     - Frequency-domain Notch filter for periodic noise
   - Reconstructs the restored image from all quadrants.

4. **Artifact Reduction**
   - Uses a Gaussian low-pass filter to smooth the borders and minimize quadrant artifacts.

5. **Solar Region Segmentation**
   - Segments the restored solar image into:
     - **Coronal Holes** (dark purple)
     - **Active Regions** (bright red)
     - **Quiet Sun** (yellow-orange)

---

## 🧩 Methods Used

- Spatial Domain Filtering  
- Frequency Domain Filtering  
- Histogram Analysis  
- Noise Parameter Estimation  
- RGB Channel Decomposition  
- Image Masking and Segmentation  

---
