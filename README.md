# Enhanced JPEG Compression using Deep Residual Learning

This repository contains an implementation of **Deep Residual Learning Based Enhanced JPEG Compression**, based on the paper [*Deep Residual Learning-based Enhanced JPEG Compression in the Internet of Things*](https://doi.org/10.1109/TII.2020.2994743). This method significantly reduces the amount of transmitted data in JPEG compression while maintaining image quality using deep residual networks.

## Overview

The project implements a novel approach to JPEG compression where only 60% of the image data is transmitted, omitting most DC coefficients. A deep residual learning model is employed to recover the missing DC coefficients and reconstruct the image with minimal loss of quality.

### Key Features
- **Reduced Data Transmission**: 40% less data transmitted compared to standard JPEG.
- **DC Recovery**: Recovery of missing DC coefficients using signal processing and deep learning.
- **High Image Quality**: Achieves over 30 dB PSNR with low block artifacts.

## Architecture

1. **Sender's End**:
   - JPEG compression is applied with only AC coefficients and four corner DC coefficients transmitted, reducing transmission data.
   
2. **Receiver's End**:
   - DC coefficients are recovered using a two-step approach: first using signal processing, and then enhancing with a deep residual learning model to remove block artifacts and improve the final image quality.
pip install -r requirements.txt

