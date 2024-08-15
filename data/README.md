# Chest X-ray Dataset

This dataset contains chest X-ray images organized into three folders:

- **train:** Contains training images for model development.
- **test:** Holds images for evaluating the trained model's performance.
- **val:** Includes validation images used during training for hyperparameter tuning and early stopping.

## Data Organization

Within each folder (train, test, val), images are further categorized into two subfolders:

- **NORMAL:** Contains X-ray images of healthy lungs.
- **PNEUMONIA:** Contains X-ray images of lungs affected by pneumonia.

## Image Format

The images are in common image formats like JPEG or PNG.

## Usage

This dataset is suitable for various tasks related to chest X-ray image analysis, including:

- **Pneumonia Detection:** Building models to classify images as normal or pneumonia.
- **Image Classification:** Developing models to identify different lung conditions based on X-ray images.
- **Medical Image Analysis:** Researching and developing new techniques for analyzing medical images.

## Example Code

The provided Python code demonstrates how to:

- **Check Image Loading:** Verify that images can be loaded successfully.
- **Explore Directory Structure:** Examine the organization of the dataset.
- **Visualize Sample Images:** Display a few images from the dataset for visual inspection.

## Notes

- Ensure that the `DATA_PATH` environment variable is set correctly to point to the location of the dataset.
- The code includes error handling to gracefully handle images that cannot be loaded.
