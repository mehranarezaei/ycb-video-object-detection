# YCB-Video Object Detection

A continuous computer-vision project by Mehrana Rezaei, working exclusively with the **YCB-Video (YCB-V)** dataset. The project follows the Group 1 practical track: dataset exploration, object classification, controlled improvements, structured error analysis, CNN recognition, and full-frame object detection. Segmentation and a final integrated demo are planned extensions.

## Scope and evaluation

All practical work uses YCB-Video, including selected subsets and the YCB-V BOP-format release where used by the notebooks. No other dataset is part of this project. Classification operates on selected object crops; detection operates on full RGB frames with class labels and bounding boxes. Depth, masks, camera information, and pose annotations are explored where relevant.

Results and execution records are documented in the supplied weekly notebooks and reports. They have not been independently reproduced here. Internal splits made from BOP-source scenes are project evaluations, not official YCB-V/BOP challenge scores. Previously inspected scenes should not be described as an untouched benchmark.

## Weekly branches

Each `week-XX` branch contains this overview, that week's notebook, and its technical report at the repository root. Select a branch below to review the corresponding work.

| Week | Practical objective | Branch |
| --- | --- | --- |
| 01 | **Dataset Understanding I** — Study purpose, classes, sequences, RGB, depth, masks, boxes, camera information, and poses; no training. | [week-01](https://github.com/mehranarezaei/ycb-video-object-detection/tree/week-01) |
| 02 | **Dataset Understanding II** — Build a dataset explorer; load and visualize annotations; calculate basic statistics. | [week-02](https://github.com/mehranarezaei/ycb-video-object-detection/tree/week-02) |
| 03 | **Object Classification I** — Prepare a selected-class subset, define train/validation/test splits, and train a baseline. | [week-03](https://github.com/mehranarezaei/ycb-video-object-detection/tree/week-03) |
| 04 | **Object Classification II** — Compare controlled regularization, augmentation, optimizer, learning-rate, and tuning experiments. | [week-04](https://github.com/mehranarezaei/ycb-video-object-detection/tree/week-04) |
| 05 | **Error Analysis I** — Inspect class-wise failures, bias/variance, difficult samples, possible label issues, and data mismatch. | [week-05](https://github.com/mehranarezaei/ycb-video-object-detection/tree/week-05) |
| 06 | **Error Analysis II** — Use the failure analysis to select targeted improvement experiments and recommendations. | [week-06](https://github.com/mehranarezaei/ycb-video-object-detection/tree/week-06) |
| 07 | **CNN Classification I** — Build a clean CNN recognition baseline on the same object subset and compare earlier results. | [week-07](https://github.com/mehranarezaei/ycb-video-object-detection/tree/week-07) |
| 08 | **CNN Classification II** — Explore transfer learning or a stronger CNN; study viewpoint, clutter, scale, and occlusion. | [week-08](https://github.com/mehranarezaei/ycb-video-object-detection/tree/week-08) |
| 09 | **Object Detection I** — Predict classes and boxes on full frames; handle annotations and evaluate localization with IoU. | [week-09](https://github.com/mehranarezaei/ycb-video-object-detection/tree/week-09) |
| 10 | **Object Detection II** — Study confidence thresholds, multiple objects, NMS, precision-recall behavior, and YOLO-style concepts. | [week-10](https://github.com/mehranarezaei/ycb-video-object-detection/tree/week-10) |

## Planned extensions

- **Week 11 — Object Segmentation:** use YCB masks for pixel-level regions; evaluate IoU and boundary failures.
- **Week 12 — Final Object Understanding Demo:** integrate the strongest classification, detection, and segmentation components; compare unseen YCB examples and document limitations.

Weeks 11 and 12 are a roadmap only; this repository currently provides weekly submissions for weeks 01–10.

## Working with the notebooks

1. Select the desired weekly branch and open its `.ipynb` file in Jupyter or Google Colab.
2. Review the setup cells and install the dependencies required by that notebook.
3. Obtain the YCB-Video data needed for that experiment and configure local or Colab paths. Dataset archives and model checkpoints are not included.
4. Run the cells in order and read the accompanying report for settings, results, and limitations. Later weeks may require outputs or checkpoints produced in earlier weeks; inspect the notebook paths before running.

## Report format

Each report records the objective, relevant concepts, method and dataset subset, implementation, experimental settings, results, failure analysis, conclusions, and proposed next steps. Keep experiment settings and splits explicit so weekly comparisons are meaningful.

The weekly plan above adapts only the Group 1 practical dataset track from the supplied project brief.
