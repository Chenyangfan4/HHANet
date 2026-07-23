# HHANet

Official repository for:

**HHANet: Hybrid-Dimension Network with Height-Aware Attention for Vertebrae Detection in Routine Lumbar Spine MR Images**

This repository contains the official implementation of HHANet, an end-to-end vertebra detection framework designed for routine 3D lumbar spine magnetic resonance (MR) images.

> **Repository Status**
>
> The source code is currently under preparation and will be publicly released upon publication of the associated manuscript.

---

## Overview

Accurate vertebra detection is an important preprocessing step for downstream spine analysis tasks, including vertebral measurement, registration, and quantitative assessment.

HHANet is designed to address the challenges of routine spine MR images, including:

- strong inter-vertebral appearance similarity;
- pathological and acquisition-related anatomical variations;
- anisotropic voxel spacing with high in-plane resolution and high slice thickness;
- limited 3D contextual information caused by sparse inter-slice resolution.

The framework integrates three major components:

1. **Anisotropic Feature Extraction**

   An anisotropic backbone is introduced to better exploit the characteristics of routine spine MR images by emphasizing high-resolution in-plane structures while efficiently incorporating through-plane information.

2. **Projection-based Adaptive Feature Pyramid Network (Projection-AFPN)**

   Projection-AFPN performs efficient multi-scale feature fusion by aggregating depth-wise information and reducing redundant volumetric computation.

3. **Height-Attention Detection Head (HA-Head)**

   HA-Head incorporates anatomical height relationships among vertebral levels to improve vertebral identification and localization consistency.

HHANet provides a fully convolutional one-stage solution for vertebra localization and identification.

---

## Method Overview

The overall pipeline consists of:
