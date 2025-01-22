# Image Compression and Restoration

This repository contains two projects related to image compression techniques:
1. **JPEG Compression Engine**: A custom implementation inspired by the JPEG compression algorithm.
2. **Edge-Based Image Compression**: An implementation of a research paper that employs edge detection and homogeneous diffusion for image compression.

[Click here](CS663_Project_Report.pdf) for the detailed project report summarizing the methods, experiments, and results.

---

## Repository Contents
- **`JPEG_compression_engine.ipynb`**: Implements a JPEG-like compression algorithm.
- **`Research_Paper_Implementation.ipynb`**: Implements edge-based image compression from a research paper ([link to paper](https://projet.liris.cnrs.fr/imagine/pub/proceedings/CAIP-2009/papers/5702/57020476.pdf)).
- **`CS663_Project_Report.pdf`**: Comprehensive report detailing methodologies, experiments, and results of both projects.

---

## Features

### 1. JPEG Compression Engine
- **Techniques Used**:
  - **Discrete Cosine Transform (DCT)**: Converts image data from spatial to frequency domain.
  - **Quantization**: Reduces precision for compression.
  - **Huffman Encoding**: Entropy coding for efficient data representation.
  ![Workflow Diagram](path/to/sample_graph.png)
- **Objectives**:
  - Implement core JPEG compression steps for grayscale images.
  - Evaluate compression with metrics such as **Bits Per Pixel (BPP)** and **Root Mean Squared Error (RMSE)**.
  - Simulate varying quality factors and plot **RMSE vs. BPP** curves.
- **Sample Results**:
  ![RMSE vs BPP Curve](path/to/sample_graph.png)
  ![Sample Compression](path/to/compressed_images.png)

### 2. Edge-Based Image Compression
- **Stages**:
  - **Edge Detection and Mask Generation**: Identifies edges for efficient compression.
  - **Subsampling**: Reduces redundant data storage near edges.
  - **Supersampling**: Improves reconstruction near edges.
  - **Reconstruction**: Uses homogeneous diffusion to fill missing data.
- **Sample Workflow**:
  ![Workflow Diagram](path/to/flowchart.png)
- **Sample Results**:
  ![Edge-Based Compression](path/to/edge_compression_results.png)

---

## Installation and Usage

### Prerequisites
- Python 3.8 or above
- Required libraries:
  - `numpy`
  - `opencv-python`
  - `scipy`
  - `matplotlib`
  - `jupyterlab`

Install dependencies using:
```bash
pip install numpy opencv-python scipy matplotlib jupyterlab
```

### Execution
Clone the repository:
```bash
git clone https://github.com/username/repo-name.git
cd repo-name
```

Run the notebooks:
1. Open `JPEG_compression_engine.ipynb` or `Research_Paper_Implementation.ipynb` in Jupyter Lab/Notebook.
2. Execute cells sequentially to see results and visualizations.

## Results and Analysis

### JPEG Compression
- Significant compression achieved with minimal loss in visual quality.
- Observed inverse exponential decay of RMSE with increasing BPP.

### Edge-Based Compression
- Moderate compression rates with limitations in Peak Signal-to-Noise Ratio (PSNR) for detailed images.
- For detailed analysis, refer to `CS663_Project_Report.pdf`.

## Contributions
Feel free to contribute by opening issues or submitting pull requests. Feedback is highly appreciated!

## Acknowledgments
- Prof. Ajit Rajwade, Indian Institute of Technology Bombay.
- Research paper authors for their innovative methods in image compression.
- Libraries: NumPy, OpenCV, SciPy, and Matplotlib.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

---

### Notes
- Replace `path/to/sample_graph.png`, `path/to/compressed_images.png`, and `path/to/flowchart.png` with actual paths to images or screenshots from your project.
- Add any additional results or insights if available.
