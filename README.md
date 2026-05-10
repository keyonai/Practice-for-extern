# Image Preprocessing — OpenCV Document Enhancement

Applied image preprocessing techniques to clean up a noisy scanned document using OpenCV. Demonstrates a real-world preprocessing pipeline that improves image quality before feeding into OCR or computer vision models.

## What it does

- Loads a noisy scanned document image
- Applies denoising to remove background noise
- Enhances contrast to make text more legible
- Uses thresholding to produce a clean black-and-white output
- Saves and displays the processed result

## Stack

- Python
- OpenCV
- Jupyter Notebook

## Setup

```bash
pip install opencv-python numpy matplotlib
```

## Usage

Open `Keyonai_Enhance_a_Scanned_Document_Using_Preprocessing.ipynb` in Jupyter and run all cells.

Sample images are included:
- `noisy_image_sample.jpg` — raw input
- `processed_image.jpg` — cleaned output

## Preprocessing pipeline

| Step | Technique |
|------|-----------|
| Denoising | `cv2.fastNlMeansDenoising` |
| Contrast enhancement | CLAHE / histogram equalization |
| Thresholding | Otsu's binarization |
