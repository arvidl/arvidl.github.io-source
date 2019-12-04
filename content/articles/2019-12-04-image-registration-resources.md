Title: Image registration resources <small></small>
date: 2019-12-04
comments: true
slug: image-registration-resources
tags: data, numpy, matplotlib, pandas, scipy, scikit-learn, scikit-image, nibabel, jupyter, keras, tensorflow, pytorch


#### See  [[Jupyter notebooks for learning how to use SimpleITK](https://github.com/InsightSoftwareConsortium/SimpleITK-Notebooks)]

-----------------------------------------------

## 3D image registration  ([pyimreg](http://pyimreg.github.io)) ([image-registration](https://github.com/topics/image-registration))


- [**Medical Image Registration Tutorial**](https://github.com/natandrade/Tutorial-Medical-Image-Registration)<br>
A practical review on medical image registration: from rigid to deep learning based approaches.

- [**Learn2Reg 2019**](https://github.com/learn2reg/tutorials2019)<br>
MICCAI 2019 [Tutorial](https://learn2reg.github.io) on Deep Learning in Medical Image Registration.

- [**SimpleITK**](https://github.com/SimpleITK)<br>
SimpleITK: a simplified layer build on top of the Insight Toolkit (ITK), intended to facilitate its use in rapid prototyping, education and interpreted languages.

- [**SimpleElastix**](https://simpleelastix.github.io)<br>
SimpleElastix is an extension of [SimpleITK](http://www.simpleitk.org) that includes the popular [elastix](http://elastix.isi.uu.nl) C++ library. Elastix is a modular collection of high-performance medical image registration algorithms, for which SimpleElastix automatically generates bindings for Python, Java, R, Ruby, Octave, Lua, Tcl and C#. This makes state-of-the-art registration really easy to do in your favorite programming environment.

- [**ANTsPy**](https://github.com/ANTsX/ANTsPy)<br>
ANTsPy is a Python library which wraps the C++ biomedical image processing library ANTs, matches much of the statistical capabilities of [ANTsR](https://github.com/ANTsX/ANTsR), and allows seamless integration with numpy, scikit-learn, and the greater Python community. ANTsPy includes blazing-fast IO (~40% faster than nibabel for loading Nifti images and converting them to numpy arrays), registration, segmentation, statistical learning, visualization, and other useful utility functions.

   - *ANTsR installation* with devtools in R<br>
 `library(devtools)`<br>
 `install_github("stnava/cmaker")` # if you do not have cmake<br>
 `install_github("stnava/ANTsR")`

   - [Anatomy of an antsRegistration call](https://github.com/ANTsX/ANTs/wiki/Anatomy-of-an-antsRegistration-call)<br>




- [**ANTsPyNet**](https://github.com/ANTsX/ANTsPyNet)<br>
Medical image analysis framework merging [ANTsPy](https://github.com/ANTsX/ANTsPy) and deep learning

  - *[ANTsRNET](https://github.com/ANTsX/ANTsRNet) installation* with devtools in R<br>
A collection of deep learning architectures ported to the R language and tools for basic medical image processing. Based on keras and tensorflow with cross-compatibility with our python analog ANTsPyNet.<br>
 `library(devtools)`<br>
 `devtools::install_github("ANTsX/ANTsRNet")`

- [**Pirt**](https://pirt.readthedocs.io)<br>
Pirt is the “Python image registration toolkit”. It is a library for (elastic, i.e. non-regid) image registration of 2D and 3D images with support for groupwise registration. It has support to constrain the deformations to be “diffeomorphic”, i.e. without folding or shearing, and thus invertable. Pirt is written in pure Python and uses Numba for speed. It depends on Numpy, Scipy, Numba. It has an optional dependency on Visvis for visualization. Pirt implements its own interpolation functions, which, incidentally, are faster than the corresponding functions in scipy and scikit-image (after Numba’s JIT warmup). The functionality inside Pirt is implemented over a series of submodules, but (almost) all functions and classes are available in the main namespace. (*Not updated since September 2017*)

- [**voxelmorph**](https://github.com/voxelmorph/voxelmorph)<br>
Unsupervised Learning with CNNs for Image Registration. This repository incorporates several variants, first presented at CVPR2018 (initial unsupervised learning) and then MICCAI2018 (probabilistic & diffeomorphic formulation).

- [**cnn-registration**](https://github.com/yzhq97/cnn-registration)<br>
A image registration method using convolutional neural network features.

- [**airlab**](https://github.com/airlab-unibas/airlab)<br>
AirLab is an open laboratory for medical image registration (2D and 3D image data). It provides an environment for rapid prototyping and reproduction of registration algorithms. The unique feature of AirLab is, that the analytic gradients of the objective function are computed automatically with fosters rapid prototyping. In addition, the device on which the computations are performed, on a CPU or a GPU, is transparent. AirLab is implemented in Python using PyTorch as tensor and optimization library and SimpleITK for basic image IO. It profits therefore from recent advances made by the machine learning community.  See [arXiv preprint 2018](https://arxiv.org/abs/1806.09907) for a detailed introduction of AirLab and its feature.

- [**RegNet**](https://github.com/hsokooti/RegNet)<br>
Nonrigid image registration using multi-scale 3D convolutional neural networks.

- [**istn**](https://github.com/biomedia-mira/istn)<br>
Image-and-Spatial Transformer Networks. Introduces a novel, generic, learning-based image registration framework, Image-and-Spatial Transformer Networks, to leverage Structures-of-Interest information allowing to learn new image representations that are optimised for the downstream registration task. Thanks to these representations one can employ a test-specific, iterative refinement over the transformation parameters which yields highly accurate registration even with very limited training data.

- [**BIRL**](https://github.com/Borda/BIRL)<br>
BIRL: Benchmark on Image Registration methods with Landmark validations http://borda.github.io/BIRL. This project/framework is the key component of Automatic Non-rigid Histological Image Registration (ANHIR) challenge hosted at ISBI 2019 conference. The task consists of registering multi-stain histology images. The related discussion is hosted on [forum.image.sc](https://anhir.grand-challenge.org)

- [**lagomorph**](https://github.com/jacobhinkle/lagomorph)<br>
Image Registration and Computational Anatomy in PyTorch. Lagomorph aims to provide tools for [computational anatomy](https://en.wikipedia.org/wiki/Computational_anatomy) in the context of the deep learning framework PyTorch, which will enable easier integration of image registration methodologies with deep learning.


-- **REFERENCES** --

G. Haskins, U. Kruger, P. Yan: **Deep Learning in Medical Image Registration: A Survey** [[arXiv:1903.02026](https://arxiv.org/abs/1903.02026)]<br>
*The establishment of image correspondence through robust image registration is critical to many clinical tasks such as image fusion, organ atlas creation, and tumor growth monitoring, and is a very challenging problem. Since the beginning of the recent deep learning renaissance, the medical imaging research community has developed deep learning based approaches and achieved the state-of-the-art in many applications, including image registration. The rapid adoption of deep learning for image registration applications over the past few years necessitates a comprehensive summary and outlook, which is the main scope of this survey. This requires placing a focus on the different research areas as well as highlighting challenges that practitioners face. This survey, therefore, outlines the evolution of deep learning based medical image registration in the context of both research challenges and relevant innovations in the past few years. Further, this survey highlights future research directions to show how this field may be possibly moved forward to the next level.*

--**CHALLENGES**--

- [**Continuous Registration Challenge**](https://continuousregistration.grand-challenge.org) (CRC) is a challenge for registration of lung- and brain images inspired by modern software development practices.

- [**ANHIR**](https://anhir.grand-challenge.org)  Automatic Non-rigid Histological Image Registration (ANHIR) challenge. In digital pathology, it is often useful to align spatially close but differently stained tissue sections in order to obtain the combined information. The images are large, in general, their appearance and their local structure are different, and they are related through a nonlinear transformation. The proposed challenge focuses on comparing the accuracy and approximative speed of automatic non-linear registration methods for this task. Registration accuracy will be evaluated using manually annotated landmarks. All methods are supposed to run fully automatically, with no image specific parameters. Part of the IEEE International Symposium on Biomedical Imaging (ISBI) 2019 [challenges](https://biomedicalimaging.org/2019/challenges).

-- **List of medical imaging** [**datasets**](https://github.com/adalca/medical-datasets) <br>
  - [Medical Data for Machine Learning](https://github.com/beamandrew/medical-data)


{% notebook downloads/notebooks/ImageRegistrationResources.ipynb cells[2:] %}
