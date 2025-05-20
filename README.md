
# Solar Flare Detection in AIA 1600 Images Using YOLOv8

**This repository contains the implementation of an object detection system for solar flares using YOLOv8.**
The solution is designed to identify flare ribbon locations in AIA 1600 Å images provided by NASA’s Solar Dynamics Observatory (SDO).

The model is trained on flare event data from RibbonDB and supports visualization and evaluation of detection results.

---

### Repository contains:

* **final.ipynb** – complete notebook with the full pipeline, including data preparation, image loading, label generation, model prediction, evaluation, and visualization. All sections include detailed comments and explanations.

* **best.pt** – trained YOLOv8 model used for inference.

* **custom_data.yaml** – configuration file defining class names and dataset structure for training the YOLO model.

* **ribbondb_v1.0.csv** – catalog of solar flare events (start/end time, coordinates, region ID, etc.), used for retrieving SDO images and generating labels.  
  **Source**: [Kazachenko RibbonDB](https://solarmuri.ssl.berkeley.edu/~kazachenko/RibbonDB/)



This implementation is part of a bachelor’s thesis at the **Technical University of Košice**.
