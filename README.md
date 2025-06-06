## Surface3D: A Surface-Aware Framework for Refining 3D Object Detection

[Mingyu Liu](https://scholar.google.com/citations?user=Bcohc-oAAAAJ), Yutong Hou, [Ekim Yurtsever](https://scholar.google.com/citations?hl=zh-CN&user=dJGmJCEAAAAJ), [Xingcheng Zhou](https://scholar.google.com/citations?hl=zh-CN&user=FPYXLpQAAAAJ), [Haolin Zhang](https://scholar.google.com/citations?hl=zh-CN&user=odp2WtkAAAAJ), [Jiajie Zhang](https://www.ce.cit.tum.de/air/people/jiajie-zhang-msc/), and [Alois C. Knoll](https://scholar.google.com/citations?hl=zh-CN&user=-CA8QgwAAAAJ&view_op=list_works)

>**Abstract:** 3D object detection aims to identify objects and localize them by predicting bounding boxes from LiDAR point clouds.} However, the inherent sparsity of LiDAR data, partial occlusions, and challenges posed by long-tail viewing angles often limit their performance. To address these limitations, we propose Surface3D, a surface-aware refinement approach that integrates learned surface features derived from part segmentation to enhance bounding box predictions. \added{Existing datasets primarily focus on indoor scene segmentation and are not suitable for our task. To address this, we develop a semi-automated pipeline to generate training data for part segmentation. This module extracts object surface features from the initial detection outputs. A refinement module then leverages these features to improve the accuracy of bounding box sizes and orientations. Extensive experiments on the KITTI dataset using five widely adopted 3D object detectors demonstrate that incorporating surface features substantially improves detection performance. Our approach improves 3D object detection performance across five detectors on KITTI. Specifically, it achieves up to 1.75\% and 1.25\% gains over PointPillars and VoxelRCNN, respectively, on the hard car class under 3D AP_{R11} metrics.

### Network Architecture
<img src="/figures/pipeline.png">

### Data Generation Pipeline and Examples of Generaterd 2D/3D Data
<details close>
<summary><b>Data Generation Pipeline:</b></summary>

![results1](/figures/3D_data_gen_pipeline.png)
</details>

<details close>
<summary><b>2D Segmentation Data:</b></summary>

![results1](/figures/2D_seg_results.png)
</details>

<details close>
<summary><b>3D Segmentation Data:</b></summary>

![results1](/figures/3D_seg_results.png)
</details>

### Experimental results
<details close>
<summary><b>Quantitative Results on the KITTI Validation Set:</b></summary>

![results1](/figures/quantitative_res.png)
</details>

<details close>
<summary><b>Qualitatitve Results:</b></summary>

![results1](/figures/qualitative_res.png)
</details>
