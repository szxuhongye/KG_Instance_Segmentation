# KG_Instance_Segmentation
Multi-scale Cell Instance Segmentation with Keypoint Graph based Bounding Boxes

Please cite the article in your publications if it helps your research:

	@inproceedings{YI2019MICCAI,
		author = "Jingru Yi and Pengxiang Wu and Qiaoying Huang and Hui Qu and Bo Liu and Daniel J. Hoeppner and Dimitris N. Metaxas"
		title = "Multi-scale Cell Instance Segmentation with Keypoint Graph based Bounding Boxes",
		booktitle = "MICCAI",
		year = "2019",
	}

# Introduction

Most existing methods handle cell instance segmentation
problems directly without relying on additional detection boxes. This
method generally fails to separate touching cells due to the lack of global
understanding of the objects. In contrast, box-based instance segmenta-
tion solves this problem by combining object detection with segmenta-
tion. However, existing methods typically utilize anchor box-based de-
tectors, which would lead to inferior instance segmentation performance
due to the class imbalance issue. In this paper, we propose a new box-
based cell instance segmentation method. In particular, we first detect
the five pre-defined points of a cell via keypoints detection. Then we
group these points according to a keypoint graph and subsequently ex-
tract the bounding box for each cell. Finally, cell segmentation is per-
formed on feature maps within the bounding boxes. We validate our
method on two cell datasets with distinct object shapes, and empirically
demonstrate the superiority of our method compared to other instance
segmentation techniques.

<p align="center">
	<img src="imgs/pic1.png", width="800">
</p>


# Dependencies
Ubuntu 14.04, python 3.6.4, pytorch 1.1.0, opencv-python 4.1.0.25 
