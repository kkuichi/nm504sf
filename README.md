
# Solar Flare Detection in AIA 1600 Images Using YOLOv8

**This repository contains the implementation of an object detection system for solar flares using YOLOv8.**
The solution is designed to identify flare ribbon locations in AIA 1600 Å images provided by NASA’s Solar Dynamics Observatory (SDO).

The model is trained on flare event data from RibbonDB and supports visualization and evaluation of detection results.

---

### Repository contains:

* **final.ipynb** – a complete notebook with the full pipeline, including data preparation, image loading, label generation, model training, prediction, evaluation, and visualization. The file also includes code for training the model, and a pre-trained model ready for use is also provided. All sections contain detailed comments and explanations.

* **best.pt** – the trained YOLOv8 model used for inference. The model was trained using custom parameters provided in this repository and took 5 days to train on a Quadro RTX 4000.

* **custom_data.yaml** – Configuration file defining class names and dataset structure for training the YOLO model. The parameters were selected based on the specific characteristics of the data, aiming to enhance and augment the existing dataset.

* **ribbondb_v1.0.csv** – catalog of solar flare events (start/end time, coordinates, region ID, etc.), used for retrieving SDO images and generating labels.  
  **Source**: [Kazachenko RibbonDB](https://solarmuri.ssl.berkeley.edu/~kazachenko/RibbonDB/)



This implementation is part of a bachelor’s thesis at the **Technical University of Košice**.
