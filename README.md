# Awesome Hand Pose Estimation [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of awesome hand pose estimation papers, frameworks, libraries, software and resources.

- [Awesome Hand Pose Estimation](#awesome-hand-pose-estimation)
  - [Papers](#papers)
    - [Monochrome RGB-based Pose Estimation](#monochrome-rgb-based-pose-estimation)
    - [Video-based Pose Estimation](#video-based-pose-estimation)
    - [Hand Reconstruction](#hand-reconstruction)
    - [Hand Object Interaction](#hand-object-interaction)
  - [Hand Models](#hand-models)
  - [Datasets](#datasets)
  - [Contributing](#contributing)

## Papers

### Monochrome-based Hand Pose Estimation
* [2020 SIGGRAPH] MEgATrack: Monochrome Egocentric Articulated Hand-Tracking for Virtual Reality. [\[PDF\]](https://dl.acm.org/doi/abs/10.1145/3386569.3392452)

### RGB-based Hand Pose Estimation
* [2017 ICCV] Learning to Estimate 3D Hand Pose from Single RGB Images. [\[PDF\]](https://arxiv.org/pdf/1705.01389.pdf)  [\[Project\]](https://lmb.informatik.uni-freiburg.de/projects/hand3d/)   [\[Code\]](https://github.com/lmb-freiburg/hand3d)

*  [2019 CVPR] 3D Hand Shape and Pose Estimation from a Single RGB Image. [\[PDF\]](http://openaccess.thecvf.com/content_CVPR_2019/papers/Ge_3D_Hand_Shape_and_Pose_Estimation_From_a_Single_RGB_CVPR_2019_paper.pdf) [\[Project\]](https://sites.google.com/site/geliuhaontu/home/cvpr2019) [\[Code\]](https://github.com/3d-hand-shape/hand-graph-cnn) *(Oral)*
_Liuhao Ge, Zhou Ren, Yuncheng Li, Zehao Xue, Yingying Wang, Jianfei Cai, Junsong Yuan_

### Video-based Hand Pose Estimation

* SeqHAND: RGB-Sequence-Based 3D Hand Pose and Shape Estimation. [\[PDF\]](http://arxiv.org/pdf/2007.05168)
_John Yang, Hyung Jin Chang, Seungeui Lee, Nojun Kwak_

### Triangulation
* [2019 ICCV] Learnable Triangulation of Human Pose. [\[PDF\]](https://arxiv.org/pdf/1905.05754.pdf) [\[Project\]](https://saic-violet.github.io/learnable-triangulation/) [\[Code\]](https://github.com/karfly/learnable-triangulation-pytorch#learnable-triangulation-of-human-pose) *(Oral)*
_Karim Iskakov, Egor Burkov, Victor Lempitsky, Yury Malkov_

* [2020 CVPR] Epipolar Transformers. [\[PDF\]](https://arxiv.org/pdf/2005.04551.pdf) [\[Code\]](https://github.com/yihui-he/epipolar-transformers)
_Yihui He\*, Rui Yan\*, Shoou-I Yu, Katerina Fragkiadaki_

### Hand Reconstruction

* [2020 CVPR] Weakly-Supervised Mesh-Convolutional Hand Reconstruction in the Wild. [\[PDF\]](https://arxiv.org/pdf/2004.01946.pdf) [\[Project\]](https://www.arielai.com/mesh_hands/)  *(Oral)* *([Paper Award Nominees](http://cvpr2020.thecvf.com/node/817))* _Dominik Kulon, Riza Alp Güler, Iasonas Kokkinos, Michael Bronstein, Stefanos Zafeiriou_

### Hand Object Interaction
* H+O: Unified Egocentric Recognition of 3D Hand-Object Poses and Interactions. [\[PDF\]](https://openaccess.thecvf.com/content_CVPR_2019/papers/Tekin_HO_Unified_Egocentric_Recognition_of_3D_Hand-Object_Poses_and_Interactions_CVPR_2019_paper.pdf)
_Bugra Tekin, Federica Bogo, Marc Pollefeys_

### Body Pose Estimation
* [2020 ECCV] Whole-Body Human Pose Estimation in the Wild. [\[PDF\]](https://arxiv.org/pdf/2007.11858.pdf) [\[Code\]](https://github.com/jin-s13/COCO-WholeBody)
_Sheng Jin, Lumin Xu, Jin Xu, Can Wang, Wentao Liu, Chen Qian, Wanli Ouyang, Ping Luo_

---

## Hand Models
* Manopth [\[Project\]](https://github.com/hassony2/manopth)

## Datasets
- S/R: Synthetic (S) or Real (R) or Both (B)
- C/D: Color (RGB) or Depth (D)
- Obj: Interaction with objects or not
- #J:  No. of joints or Mesh (M)
- V: view (3rd or egocentric)
- #S: No. of subjects
- #F: No. of frames (train/test)
- Mesh: Mesh annotations

### Depth

|Dataset|Year|S/R|Mesh|Obj|#J|V|#S|#F|Paper|
|------|------|------|------|------|------|------|------|------|----------------|
|[NYU](http://cims.nyu.edu/~tompson/NYU_Hand_Pose_Dataset.htm) | 2014 | R |❌|❌| 36 | 3rd | 2 | 72k/8k | SIGGRAPH 2014 [\[PDF\]](http://cims.nyu.edu/~tompson/others/TOG_2014_paper_PREPRINT.pdf)|
|[ICVL](https://labicvl.github.io/hand.html) | 2014 | R |❌|❌|  16 | 3rd  |  10 | 331k/1.5k | CVPR 2014 [\[PDF\]](https://labicvl.github.io/docs/pubs/Danny_CVPR_2014.pdf)|
|[MSRA15](https://github.com/geliuhao/CVPR2016_HandPoseEstimation/issues/4) | 2015 | R |❌|❌|  21 | 3rd  |  9 | 76,375 | CVPR 2015 [\[PDF\]](http://www.cv-foundation.org/openaccess/content_cvpr_2015/papers/Sun_Cascaded_Hand_Pose_2015_CVPR_paper.pdf)|
|[BigHand2.2M](http://icvl.ee.ic.ac.uk/hands17/challenge/) | 2017 | R |❌|❌|  21 | 3rd  |  10 | 2.2M | CVPR 2017 [\[PDF\]](https://labicvl.github.io/docs/pubs/Shanxin_CVPR_2017.pdf)|
|[SynHandEgo](https://bit.ly/2WMWM5u) | 2019 | R |✅|❌| - | ego | - | - | Computers & Graphics 2019 [\[PDF\]](https://www.dfki.de/fileadmin/user_upload/import/10684_CAG_Jameel.pdf)|
|[FHAD](https://guiggh.github.io/publications/first-person-hands/) | 2018 | R |❌| ✅ |  21 | ego  |  6 | 100k | CVPR 2018 [\[PDF\]](https://arxiv.org/pdf/1704.02463)|
|[SynHand5M](https://cloud.dfki.de/owncloud/index.php/s/iCMRF7a5FkXrdpn) | 2018 | S | - |❌|  M | 3rd  |  - | 5M | 3DV 2018 [\[PDF\]](https://arxiv.org/pdf/1808.09208.pdf)|
|[MSRC (FingerPaint)](https://www.microsoft.com/en-us/download/details.aspx?id=52288)  | 2015| S |❌|❌|  21 | both  |  1 | 100k | CHI 2015 [\[PDF\]](http://www.cs.toronto.edu/~jtaylor/papers/CHI2015-HandTracking.pdf)|
|[HandNet](http://www.cs.technion.ac.il/~twerd/HandNet/) | 2015 | R |❌|❌|  6 | 3rd  |  10 | 202k/10k  | BMVC 2015 [\[PDF\]](http://www.cs.technion.ac.il/~twerd/WetzlerSlossbergKimmel-BMVC15.pdf)|
|[Hands in Action](http://files.is.tue.mpg.de/dtzionas/Hand-Object-Capture/) | 2014 | R | - | ✅ |  - | 3rd  |  - | - | IJCV 2016 [\[PDF\]](http://files.is.tue.mpg.de/dtzionas/Hand-Object-Capture/IJCV_Hand_Object_Capture.pdf)|
|[MSRA14](https://jimmysuen.github.io/) | 2014|  R |❌|❌|  21 | 3rd  |  6 | 2,400 | CVPR 2014 [\[PDF\]](http://www.cv-foundation.org/openaccess/content_cvpr_2014/papers/Qian_Realtime_and_Robust_2014_CVPR_paper.pdf)|
|[ASTAR](http://hpes.bii.a-star.edu.sg/) | 2013 | R | - |❌|  20 | 3rd  |  30 | 870 | ICCV 2013 [\[PDF\]](http://www.cv-foundation.org/openaccess/content_iccv_2013/papers/Xu_Efficient_Hand_Pose_2013_ICCV_paper.pdf)|


### RGB+Depth

|Dataset|Year|S/R|Mesh|Obj|#J|V|#S|#F|Paper|
|------|------|------|------|------|------|------|------|------|----------------|
|[ContactPose](https://contactpose.cc.gatech.edu/) | 2020 | R | ✅ | ✅ | 21 | 3rd | 50 | 2.9M | ECCV 2020 [\[PDF\]](http://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123580358.pdf)|
|[Ego3DHands](https://github.com/AlextheEngineer/Ego3DHands) | 2020 | S | - |❌| 21 | ego | 1 | 50k/5k | arXiv 2020 [\[PDF\]](https://arxiv.org/pdf/2006.01320.pdf)|
|[ObMan](https://www.di.ens.fr/willow/research/obman/data/) | 2019 | S | ✅ |✅| - | - | - | 150k | CVPR 2019 [\[PDF\]](https://openaccess.thecvf.com/content_CVPR_2019/papers/Hasson_Learning_Joint_Reconstruction_of_Hands_and_Manipulated_Objects_CVPR_2019_paper.pdf)|
|[EgoDexter](http://handtracker.mpi-inf.mpg.de/projects/OccludedHands/EgoDexter.htm) | 2017 | R | - | ✅ |  5 | ego  |  4 | 1485 | ICCV 2017 [\[PDF\]](http://handtracker.mpi-inf.mpg.de/projects/OccludedHands/content/OccludedHands_ICCV2017.pdf)|
|[SynthHands](http://handtracker.mpi-inf.mpg.de/projects/OccludedHands/SynthHands.htm) | 2017 | S | - | Both |  21 | ego  |  2 | 63,530  | ICCV 2017 [\[PDF\]](http://handtracker.mpi-inf.mpg.de/projects/OccludedHands/content/OccludedHands_ICCV2017.pdf)|
|[RHD](https://lmb.informatik.uni-freiburg.de/resources/datasets/RenderedHandposeDataset.en.html) | 2017 | S | - |❌|  21 | 3rd  |  20 | 41k/2.7k  |ICCV 2017 [\[PDF\]](https://arxiv.org/pdf/1705.01389.pdf)|
|[STB](https://sites.google.com/site/zhjw1988/) | 2017 | R | - |❌|  21 | 3rd |  1 | 18k | ICIP 2017 [\[PDF\]](http://www.cs.cityu.edu.hk/~jianbjiao2/pdfs/icip.pdf)|
|[Dexter+Object](http://handtracker.mpi-inf.mpg.de/projects/RealtimeHO/dexter+object.htm) | 2016 | R | - | ✅ |  5 | 3rd  |  2 | 3,014 | ECCV 2016 [\[PDF\]](http://handtracker.mpi-inf.mpg.de/projects/RealtimeHO/content/RealtimeHO_ECCV2016.pdf)|
|[UCI-EGO](http://pascal.inrialpes.fr/data2/grogez/UCI-EGO/UCI-EGO.tar.gz) | 2014 | R |-|❌|  26 | ego  |  2 | 400 | ECCVW 2014 [\[PDF\]](https://www.cs.cmu.edu/~deva/papers/egocentric_depth_workshop.pdf)|
|[Dexter1](http://handtracker.mpi-inf.mpg.de/projects/handtracker_iccv2013/dexter1.htm) | 2013 | R |- |❌|  6 | 3rd |  1 | 2,137 | ICCV 2013 [\[PDF\]](http://handtracker.mpi-inf.mpg.de/projects/handtracker_iccv2013/content/handtracker_iccv2013.pdf)|

### RGB

|Dataset|Year|S/R|Mesh|Obj|#J|V|#S|#F|Paper|
|------|------|------|------|------|------|------|------|------|----------------|
|[InterHand2.6M](https://mks0601.github.io/InterHand2.6M/) | 2020 | R | ❌ | ❌ | 21 | 3rd | 27 | 2.6M | ECCV 2020 [\[PDF\]](http://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123650545.pdf)|
|[YouTube 3D Hands](https://github.com/arielai/youtube_3d_hands) | 2020 | R | ✅ | ✅ | - | 3rd | - | 47,125/1525/1525 | CVPR 2020 [\[PDF\]](https://openaccess.thecvf.com/content_CVPR_2020/papers/Kulon_Weakly-Supervised_Mesh-Convolutional_Hand_Reconstruction_in_the_Wild_CVPR_2020_paper.pdf)|
|[OneHand10K](https://yangangwang.com/papers/WANG-MCC-2018-10.html) | 2019 | R | - |❌| 21 | 3rd | 1 | 10k/1.3k | TCSVT 2019 [\[PDF\]](https://yangangwang.com/papers/WANG-MCC-2018-10.pdf)|
|[FreiHAND](https://lmb.informatik.uni-freiburg.de/resources/datasets/FreihandDataset.en.html) | 2019 | R | - | ✅ |  21 | 3rd  |  - | 130k/3960  | ICCV 2019 [\[PDF\]](https://arxiv.org/pdf/1909.04349.pdf)|
|[GANerated Hands](https://handtracker.mpi-inf.mpg.de/projects/GANeratedHands/GANeratedDataset.htm) | 2018 | S | - | Both |  21 | ego  |  - | 330k | CVPR 2018 [\[PDF\]](https://handtracker.mpi-inf.mpg.de/projects/GANeratedHands/content/GANeratedHands_CVPR2018.pdf)|
|[CMU Panoptic HandDB](http://domedb.perception.cs.cmu.edu/handdb.html) | 2017 | B | - |❌|  21 | 3rd  |  - | 14,817 | CVPR 2017 [\[PDF\]](https://arxiv.org/pdf/1704.07809)|
|[MHP](http://www.rovit.ua.es/dataset/mhpdataset/) | 2017 | R | - | ❌  | 21 | 3rd | 9 | 80k | IVC 2017 [\[PDF\]](https://arxiv.org/pdf/1707.03742.pdf)  |

**Credits:**
- [1] Big Hand 2.2M Benchmark: Hand Pose Data Set and State of the Art Analysis, CVPR 2017 [\[PDF\]](https://labicvl.github.io/docs/pubs/Shanxin_CVPR_2017.pdf)
- [2] Depth-based hand pose estimation: methods, data, and challenges, ICCV 2015  [Link](http://arrummzen.net/#HandData)
- [3] Capturing Hand-Object Interaction and Reconstruction of Manipulated Objects, IJCV 2016 [\[PDF\]](http://ps.is.tue.mpg.de/uploads_file/attachment/attachment/340/Thesis_FINAL_online.pdf)
- [4] [MPI Hand Tracking Central](http://handtracker.mpi-inf.mpg.de/)

## Contributing

Your contributions are always welcome! Please take a look at the [contribution guidelines](https://github.com/vinta/awesome-python/blob/master/CONTRIBUTING.md) first.

I will keep some pull requests open if I'm not sure whether those libraries are awesome, you could [vote for them](https://github.com/vinta/awesome-python/pulls) by adding :+1: to them. Pull requests will be merged when their votes reach **20**.

---

If you have any question about this opinionated list, do not hesitate to contact me [@KaiXu]() or open an issue on GitHub.
