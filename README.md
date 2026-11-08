# YCB-Video Object Detection

A continuous computer-vision project, working exclusively with the **YCB-Video (YCB-V)** dataset. The project follows these practical track: dataset exploration, object classification, controlled improvements, structured error analysis, CNN recognition, and full-frame object detection. Segmentation and a final integrated demo are planned extensions.

## Scope and evaluation

All practical work uses YCB-Video, including selected subsets and the YCB-V BOP-format release where used by the notebooks. No other dataset is part of this project. Classification operates on selected object crops; detection operates on full RGB frames with class labels and bounding boxes. Depth, masks, camera information, and pose annotations are explored where relevant.

Results and execution records are documented in the supplied weekly notebooks and reports. They have not been independently reproduced here. Internal splits made from BOP-source scenes are project evaluations, not official YCB-V/BOP challenge scores. Previously inspected scenes should not be described as an untouched benchmark.

## Weekly files and branches

All ten weeks are available together on `main` in the `week-01` through `week-10` folders. Each folder contains that week's original notebook and technical report. The separate weekly branches are also preserved.

| Week | Practical objective | Files on main | Branch |
| --- | --- | --- | --- |
| 01 | **Dataset Understanding I** — Study purpose, classes, sequences, RGB, depth, masks, boxes, camera information, and poses; no training. | [week-01](week-01/) | [week-01 branch](https://github.com/mehranarezaei/ycb-video-object-detection/tree/week-01) |
| 02 | **Dataset Understanding II** — Build a dataset explorer; load and visualize annotations; calculate basic statistics. | [week-02](week-02/) | [week-02 branch](https://github.com/mehranarezaei/ycb-video-object-detection/tree/week-02) |
| 03 | **Object Classification I** — Prepare a selected-class subset, define train/validation/test splits, and train a baseline. | [week-03](week-03/) | [week-03 branch](https://github.com/mehranarezaei/ycb-video-object-detection/tree/week-03) |
| 04 | **Object Classification II** — Compare controlled regularization, augmentation, optimizer, learning-rate, and tuning experiments. | [week-04](week-04/) | [week-04 branch](https://github.com/mehranarezaei/ycb-video-object-detection/tree/week-04) |
| 05 | **Error Analysis I** — Inspect class-wise failures, bias/variance, difficult samples, possible label issues, and data mismatch. | [week-05](week-05/) | [week-05 branch](https://github.com/mehranarezaei/ycb-video-object-detection/tree/week-05) |
| 06 | **Error Analysis II** — Use the failure analysis to select targeted improvement experiments and recommendations. | [week-06](week-06/) | [week-06 branch](https://github.com/mehranarezaei/ycb-video-object-detection/tree/week-06) |
| 07 | **CNN Classification I** — Build a clean CNN recognition baseline on the same object subset and compare earlier results. | [week-07](week-07/) | [week-07 branch](https://github.com/mehranarezaei/ycb-video-object-detection/tree/week-07) |
| 08 | **CNN Classification II** — Explore transfer learning or a stronger CNN; study viewpoint, clutter, scale, and occlusion. | [week-08](week-08/) | [week-08 branch](https://github.com/mehranarezaei/ycb-video-object-detection/tree/week-08) |
| 09 | **Object Detection I** — Predict classes and boxes on full frames; handle annotations and evaluate localization with IoU. | [week-09](week-09/) | [week-09 branch](https://github.com/mehranarezaei/ycb-video-object-detection/tree/week-09) |
| 10 | **Object Detection II** — Study confidence thresholds, multiple objects, NMS, precision-recall behavior, and YOLO-style concepts. | [week-10](week-10/) | [week-10 branch](https://github.com/mehranarezaei/ycb-video-object-detection/tree/week-10) |


## Working with the notebooks

1. Open the desired `week-XX` folder on `main` and open its `.ipynb` file in Jupyter or Google Colab. You can also use the corresponding weekly branch.
2. Review the setup cells and install the dependencies required by that notebook.
3. Obtain the YCB-Video data needed for that experiment and configure local or Colab paths. Dataset archives and model checkpoints are not included.
4. Run the cells in order and read the accompanying report for settings, results, and limitations. Later weeks may require outputs or checkpoints produced in earlier weeks; inspect the notebook paths before running.

## Report format

Each report records the objective, relevant concepts, method and dataset subset, implementation, experimental settings, results, failure analysis, conclusions, and proposed next steps. Keep experiment settings and splits explicit so weekly comparisons are meaningful.

The weekly plan above adapts only the Group 1 practical dataset track from the supplied project brief.
