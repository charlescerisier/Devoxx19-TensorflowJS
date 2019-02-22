# Devoxx19-TensorflowJS
Hold code to reproduce Devoxx19 TensorflowJS Tool in Action

This repository use jupyter notebook to create a classification model of **croissants** and **pains au chocolat**.

If you don't have Jupyter project on your machine, you can use [official docker stacks](https://github.com/jupyter/docker-stacks).

## How to run

1. Download dataset

```python
from google_images_download import google_images_download
response = google_images_download.googleimagesdownload()
response.download({"keywords":"croissant,pain au chocolat", "output_directory":"dataset"})
```

Or you can run `download_dataset.ipynb` to download images for classification.
Images will be downloaded in `dataset` folder. Please review them and remove badly classified image.

