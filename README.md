# Multiple object pose estimation in 3D from a single RGB(D) image on the NOCS dataset

This repository tracks the research papers that address the problem of estimating the pose of multiple objects in 3D from a single RGB(D) image and evaluate on the NOCS-REAL275 dataset. The repository provides a list of research papers that followed up the work presented in the paper [**Normalized object coordinate space for category-level 6D object pose and size estimation**](https://geometry.stanford.edu/projects/NOCS_CVPR2019/), a brief summary and review of the NOCS datasets, and a comparison table with results from these works on the NOCS dataset. 

Have you submitted a new manuscript or your manuscript have been accepted to a conference/journal, and your method was evaluated on the NOCS datasets?
Share the manuscript, webpage link, and results. I will include your work in this repository.

## Table of Contents

1. [List of papers](#list-of-papers)
2. [The NOCS CAMERA and REAL275 datasets](#the-nocs-camera-and-real275-datasets)
3. [Results on NOCS-REAL275](#results-on-nocs-real275)
4. [Additional references](#additional-references)
5. [Enquiries, Question and Comments](#enquiries-question-and-comments)
6. [Licence](#licence)

-------
## List of papers

The following list is not exhaustive. Note that we differentiate the links between a published *paper* and an *arxiv* submission.

[1] H. Wang, S. Sridhar, J. Huang, J. Valentin, S. Song, and L. J. Guibas, **Normalized object coordinate space for category-level 6D object pose
and size estimation**, CVPR, 2019   
[[paper](https://openaccess.thecvf.com/content_CVPR_2019/html/Wang_Normalized_Object_Coordinate_Space_for_Category-Level_6D_Object_Pose_and_CVPR_2019_paper.html)][[webpage](https://geometry.stanford.edu/projects/NOCS_CVPR2019/)][[code](https://github.com/hughw19/NOCS_CVPR2019)]

[2] D. Chen, J. Li, Z. Wang, K. Xu, **Learning Canonical Shape Space for Category-Level 6D Object Pose and Size Estimation**, CVPR, 2020  
[[paper](https://openaccess.thecvf.com/content_CVPR_2020/papers/Chen_Learning_Canonical_Shape_Space_for_Category-Level_6D_Object_Pose_and_CVPR_2020_paper.pdf)][[webpage]()][[code](https://github.com/densechen/CASS)]

[3] X. Chen, Z. Dong, J. Song, A. Geiger, O. Hilliges, **Category Level Object Pose Estimation via Neural Analysis-by-Synthesis**, ECCV 2020  
[[arxiv](https://arxiv.org/pdf/2008.08145.pdf)][[webpage](https://ait.ethz.ch/projects/2020/neural-object-fitting/)][[code](https://github.com/xuchen-ethz/neural_object_fitting)]

[4] M. Tian, M. H. Ang Jr, G. H. Lee, **Shape Prior Deformation for Categorical 6D Object Pose and Size Estimation**, ECCV 2020  
[[paper](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123660528.pdf)][[code](https://github.com/mentian/object-deformnet)]

[5] C. Wang, R. Martín-Martín, D. Xu, J. Lv, C. Lu, L. Fei-Fei, S. Savarese, Y. Zhu, **6-PACK: Category-level 6D Pose Tracker with Anchor-Based Keypoints**, ICRA 2020  
[[paper](https://ieeexplore.ieee.org/abstract/document/9196679)][[webpage](https://sites.google.com/view/6packtracking)][[code](https://github.com/j96w/6-PACK)]

[6] T. Lee, B. -U. Lee, M. Kim and I. S. Kweon, **Category-Level Metric Scale Object Shape and Pose Estimation**, in IEEE Robotics and Automation Letters, vol. 6, no. 4, pp. 8575-8582, Oct. 2021   
[[paper](https://ieeexplore.ieee.org/abstract/document/9531548)]

[7] W. Chen, X. Jia, H. J. Chang, J. Duan, L. Shen, A. Leonardis, **FS-Net: Fast Shape-based Network for Category-Level 6D Object Pose Estimation with Decoupled Rotation Mechanism**, CVPR 2021   
[[paper](https://openaccess.thecvf.com/content/CVPR2021/papers/Chen_FS-Net_Fast_Shape-Based_Network_for_Category-Level_6D_Object_Pose_Estimation_CVPR_2021_paper.pdf)][[code](https://github.com/DC1991/FS_Net)]

[8] J. Lin, Z. Wei, Z. Li, S. Xu, K. Jia, Y. Li, **DualPoseNet: Category-Level 6D Object Pose and Size Estimation Using Dual Pose Network With Refined Learning of Pose Consistency**, ICCV 2021   
[[paper](https://openaccess.thecvf.com/content/ICCV2021/papers/Lin_DualPoseNet_Category-Level_6D_Object_Pose_and_Size_Estimation_Using_Dual_ICCV_2021_paper.pdf)][[code](https://github.com/Gorilla-Lab-SCUT/DualPoseNet)]

[9] M. Z. Irshad, T. Kollar, M. Laskey, K. Stone, Z. Kira, **CenterSnap: Single-shot multi-object 3D shape reconstruction and categorical 6D pose and size estimation**, ICRA, 2022   
[[arxiv](https://arxiv.org/pdf/2203.01929.pdf)][[webpage](https://zubair-irshad.github.io/projects/CenterSnap.html)][[code](https://github.com/zubair-irshad/CenterSnap)]

[10] M. Z. Irshad, S. Zakharov, R. Ambrus, T. Kollar, Z. Kira, A. Gaidon, **ShAPO: Implicit representations for multi-object shape, appearance, and pose optimization**, ECCV, 2002  
[[arxiv](https://arxiv.org/pdf/2207.13691.pdf)][[webpage](https://zubair-irshad.github.io/projects/ShAPO.html)]


-------
## The NOCS CAMERA and REAL275 datasets

The NOCS CAMERA and REAL275 datasets were provided along with the work done by Wang et al. [1]. All the data can be downloaded [here](https://github.com/hughw19/NOCS_CVPR2019).

### Known issues
* Code and data are not provided with an open license (see [Issue#57](https://github.com/hughw19/NOCS_CVPR2019/issues/57)) and hence both code and data should be assumed under copyright. Because of this, code and data can only be forked, downloaded, and/or viewed, but not used for any other purpose. Authors declared 
that the data is only for non-commercial use; however, no license is provided when downloading the data that confirms this. 

## Results on NOCS-REAL275

The results reported in the following comparison table are taken from the corresponding papers. 

The accuracy of the detection of the 3D bounding boxes is measuring using the Jaccard Index (or Intersection over Union, IoU) at different thresholds (i.e., 25, 50, and 75 %). The accuracy of the object pose is measured using a threshold on the translation and rotation errors, and thus counting the number of objects whose pose is within the threshold over the total number of objects. For the rotation error, the thresholds are 5° and 10°. For the translation error, the thresholds are 2 cm, 5 cm, and 10 cm. The two thresholds are combined together for different evaluations.  Speed is  measured in frame per second (results were analysed and reported by FS-Net). 

_The motivation and applications behind the choices of these thresholds are not reported, and some choices seems too permissive if we consider grasping as a possible application (e.g., 5 or 10 cm, and 25% for IoU)._

Best-performing results for each column are highlighted in bold.

|Reference|IoU-25|IoU-50|IoU-75|5°,2cm|5°,5cm|5°,10cm|10°,2cm|10°,5cm|10°,10cm| Speed |
|----------|----------|----------|----------|----------|----------|----------|----------|----------|----------|--|
| [1] NOCS (32 bins)* | 84.4 | 79.3 | -- | --  | 16.1 |--| -- | 43.7 | 43.1 | 5 |
| [1] NOCS (32 bins)  | 84.8 | 78.0 | 30.1 | 7.2 | 10.0 |--| 13.8 | 25.2 | 25.8 | 5 |
| [1] NOCS (128 bins) | 84.9 | 80.5 | 30.1 | --  |  9.5 |--| --  | 26.7  | 26.7 | 5 |
| [2] [CASS](https://openaccess.thecvf.com/content_CVPR_2020/papers/Chen_Learning_Canonical_Shape_Space_for_Category-Level_6D_Object_Pose_and_CVPR_2020_paper.pdf) |84.2 | 77.7 | -- | -- | 23.5 |--| -- | 58.0 | 58.3 | -- |
| [3] [Neural-object-fitting](https://arxiv.org/pdf/2008.08145.pdf) | -- |-- | -- | -- | -- |--| -- | -- | -- | -- |
| [4] [Deformnet](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123660528.pdf) (RGB) | -- | 75.2 | 46.5 |15.7 | 18.8 |--| 33.7 | 47.4 | -- | -- |
| [4] [Deformnet](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123660528.pdf) (RGB-D) | 83.4| 77.3 | 53.2 | 19.3 | 21.4 |--| 43.2 | 54.1 | -- | 4 |
| [5] [6-Pack](https://ieeexplore.ieee.org/abstract/document/9196679) | 94.2 | -- | -- | -- | 33.3 |--| -- | -- | --| 10 |
| [6] [MSOS](https://ieeexplore.ieee.org/abstract/document/9531548) (RGB)** | 62.0 | 23.4 | 3.0 | -- | -- |--| -- | -- | 9.6 | -- |
| [6] [MSOS](https://ieeexplore.ieee.org/abstract/document/9531548) (RGB-D)** | 81.6 | 68.1 | 32.9 | -- | -- |--| -- | -- | 26.5 | -- |
| [7] [FS-Net](https://openaccess.thecvf.com/content/CVPR2021/papers/Chen_FS-Net_Fast_Shape-Based_Network_for_Category-Level_6D_Object_Pose_Estimation_CVPR_2021_paper.pdf) | **95.1** | **92.2** | 63.5 | -- | 28.2 |--| -- | 60.8 | 64.6 | **20** |
| [8] [DualPose](https://openaccess.thecvf.com/content/ICCV2021/papers/Lin_DualPoseNet_Category-Level_6D_Object_Pose_and_Size_Estimation_Using_Dual_ICCV_2021_paper.pdf) | -- | 79.8 | **62.2** | **29.3** | 35.9 |--| 50.0 | **66.8** | -- | -- |
| [9] [CenterSnap](https://arxiv.org/pdf/2203.01929.pdf) (RGB-D) | 83.5 | 80.2 | -- | -- | 27.2 |--| -- | 58.8 | 64.4 | -- |
| [9] [CenterSnap-R](https://arxiv.org/pdf/2203.01929.pdf) (RGB-D) | 83.5 | 80.2 | -- | -- | 29.1 | --|-- | 64.3 | 70.9 | -- |
| [10] [ShAPO](https://arxiv.org/pdf/2207.13691.pdf) | 85.3 | 79.0 | -- | -- | **48.8** |--| -- | **66.8** | **78.0** | -- |

*Wrong reporting from CASS  
**Different reporting of the results of the methods under comparison

Note: Authors tend to choose different thresholds when they need to compare their methods with others, and the choice often falls on more permissive thresholds as seen in many empty cells in the table. Some research papers also reports different number than the original papers, and the reason of this is not always explained. Ideally, it would be preferrable to motivate the choice behind the thresholds and evaluate on more restricitve thresholds depending on the application (e.g., grasping). 

-------
## Additional references

* E. Brachmann, A. Krull, F. Michel, S. Gumhold, J. Shotton, C. Rother, **Learning 6D Object Pose Estimation Using 3D Object Coordinates**, ECCV 2014  
[[paper](https://link.springer.com/chapter/10.1007/978-3-319-10605-2_35)]

Note: this is the first paper I am aware was defining the representation of an object as 3D object coordinates, and then estimating the object pose from this representation. NOCS seems to be inspired by this work but simply applied to Mask R-CNN as an additional branch. 

* Y. Lin, J. Tremblay, S. Tyree, P. A. Vela, S. Birchfield, **Single-stage Keypoint-based Category-level Object Pose Estimation from an RGB Image**, ICRA 2022  
[[paper](https://arxiv.org/pdf/2109.06161.pdf)]

* A. Grabner, P. M. Roth, V. Lepetit, **3D Pose Estimation and 3D Model Retrieval for Objects in the Wild**, CVPR, 2018   
[[paper](https://openaccess.thecvf.com/content_cvpr_2018/papers/Grabner_3D_Pose_Estimation_CVPR_2018_paper.pdf)][[webpage](https://www.tugraz.at/institute/icg/research/team-lepetit/research-projects/3d-pose-estimation-and-3d-model-retrieval/)]


## Enquiries, Question and Comments

If you have any further enquiries, question, or comments, or you would like to file a bug report or a feature request, use the Github issue tracker. 


## Licence

This repository is licensed under the MIT License. To view a copy of this license, see [LICENSE](LICENSE).
