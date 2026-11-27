# Cardiac CT DICOM Curation, Quality Control and Medical Image Viewer Prototype

## Project overview

This portfolio project demonstrates Python workflows for loading and inspecting a DICOM CT image, converting pixel values to Hounsfield Units (HU), applying CT windowing, preprocessing images, performing basic image analysis, and building a Jupyter Notebook-based interactive viewer prototype.

The public portfolio edition contains the independently authored notebook code and explanations. **Saved notebook execution outputs have been removed** so that dataset-derived images, metadata values, and interactive widget states are not redistributed.

## Portfolio edition and additional development materials

This is the **public portfolio edition** of the project. It intentionally contains the notebook source code and explanations without saved execution outputs or dataset files.

A fuller local development copy was retained by the author during the original research and educational work. It contains dataset-dependent execution outputs and visual demonstrations and is **not included in this public repository**. Those additional materials will only be shared if their publication is confirmed to be permitted under the applicable Stanford research-use terms and any required written permission has been obtained.

This distinction is provided for transparency: the public repository demonstrates the code and workflow, while omitting restricted dataset material. The absence of those outputs does not mean that the project was not developed or tested; it means the dataset-derived material is not being redistributed here.

## Dataset and access

The original development work used one CT DICOM image accessed through Stanford AIMI's COCA (Coronary Calcium and Chest CTs) dataset under the Stanford University School of Medicine Dataset Research Use Agreement.

The original DICOM file, dataset copies, and dataset-derived outputs are not included in this public repository. The agreement restricts distribution, publication, reproduction, and creation of derivative works without the required permission.

Anyone wishing to execute the notebooks must independently obtain authorised access to an appropriate DICOM input and comply with the applicable dataset terms. Do not use or redistribute Stanford COCA data based solely on this repository.

## Project structure

```text
Cardiac_CT_DICOM_Curation_QC_Public/
├── Notebooks/
│   ├── 01_DICOM_Metadata_Inspection.ipynb
│   ├── 02_DICOM_Image_Visualization_and_Windowing.ipynb
│   ├── 03_DICOM_Image_Preprocessing.ipynb
│   ├── 04_DICOM_Image_Processing_and_Analysis.ipynb
│   └── 05_Medical_Image_Viewer_Prototype.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

## Notebook contents

1. **DICOM Metadata Inspection** — DICOM loading, metadata inspection, pixel-array extraction, HU conversion, intensity analysis, and CT windowing.
2. **DICOM Image Visualization and Windowing** — CT window presets, window-level controls, and image visualization.
3. **DICOM Image Preprocessing** — normalization, resizing, Gaussian filtering, and CLAHE.
4. **DICOM Image Processing and Analysis** — HU thresholding, masks, edge detection, morphology, connected components, and ROI operations.
5. **Medical Image Viewer Prototype** — interactive windowing, filtering, contrast enhancement, and viewer controls.

## Technologies

- Python
- Jupyter Notebook
- NumPy
- Matplotlib
- pydicom
- SciPy
- scikit-image
- ipywidgets

## Installation

Install the listed dependencies:

```bash
pip install -r requirements.txt
```

The notebooks were developed to read a DICOM file named `IM-0001-0001.dcm` from a local `Data/` directory. That directory and its contents are intentionally not included. Check each notebook's input-path cell and adjust it for your own authorised DICOM file if necessary.

## Scope and limitations

- The prototype was developed and tested with a single 2D CT DICOM image, not a complete multi-slice series.
- DICOM series management, slice ordering, 3D reconstruction, and multiplanar reconstruction are not implemented.
- Segmentation examples use basic intensity thresholds and image-processing operations; they are not clinically validated.
- The viewer is a Jupyter Notebook prototype, not a clinical DICOM workstation.

## Data protection and permitted use

This repository contains notebook source code and explanatory text only. It does not provide the COCA dataset, original DICOM files, saved image outputs, or a download link to restricted data.

The Stanford University School of Medicine Dataset Research Use Agreement prohibits distributing, publishing, or reproducing dataset material without specific prior written permission. It also restricts derivative works. This public code-only edition therefore excludes dataset images and saved outputs. Users remain responsible for obtaining their own permissions and complying with all applicable terms.

## Disclaimer

For educational, research, and portfolio demonstration purposes only. The methods are not intended for clinical diagnosis or patient management.
