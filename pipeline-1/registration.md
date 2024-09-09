# Registration

### Why is this done?

Registration in medical image analysis is crucial for aligning images from different time points, modalities, or patients to a common coordinate system. This alignment allows for accurate comparison and integration of data, which is essential for tasks such as tracking disease progression, planning surgeries, and combining information from various imaging techniques. By ensuring that anatomical structures are consistently positioned across images, registration enhances the reliability and precision of diagnostic and therapeutic procedures. Techniques to do this are broadly classified into:

* **Rigid Registration**: Aligning images using translations and rotations.
* **Non-Rigid Registration**: Allowing for more complex deformations to align images accurately.

### How is it done?

Registration in medical image analysis typically involves the following steps:

* **Feature Detection**: Identifying key points or landmarks in the images to be aligned.
* **Transformation Model Selection**: Choosing an appropriate model (rigid, affine, or deformable) to map one image onto another.
* **Optimization**: Iteratively adjusting the transformation parameters to minimize the difference between the images.
* **Interpolation**: Estimating the intensity values at non-integer coordinates after transformation.
* **Validation**: Assessing the accuracy of the registration using metrics like mutual information or correlation.

A common problem is to identify what the optimal setting to register the images to an atlas are. They include:

* Transformation type
* Metric type
* Optimizer type
* Deep learning for image registration

### Coding Resources

* `pymia.filtering.registration`

[SimpleITK Notebook](http://insightsoftwareconsortium.github.io/SimpleITK-Notebooks/): See chapters 60-67

[ITK Software Guide, Book 2](https://itk.org/ITKSoftwareGuide/html/Book2/ITKSoftwareGuide-Book2ch3.html): This is in C++ but with a thorough description

[3D Slicer](https://www.slicer.org/): Open source software which also includes registration.

[ANTs](http://stnava.github.io/ANTs/): Advanced Normalization Tools, which come with registration algorithms.

[NiftyReg](http://cmictig.cs.ucl.ac.uk/wiki/index.php/NiftyReg): Rigid, affine and non-linear registration of medical images.

[SimpleElastix](https://simpleelastix.github.io/): An extension of SimpleITK.



TODO: also list project ideas in this component.

### References

P. Viola and W. M. I. Wells, Alignment by maximization of mutual information, Proc. IEEE Int. Conf. Comput. Vis., vol. 24, no. 2, pp. 16–23, 1995.

P. Cattin and V. Roth, Biomedical Image Analysis, 2016. \[Online]. Available: [https://miac.unibas.ch/BIA/](https://miac.unibas.ch/BIA/) \[Accessed: 08-Sep-2020].

M.-M. Rohé, M. Datar, T. Heimann, M. Sermesant, and X. Pennec, “SVF-Net: Learning Deformable Image Registration Using Shape Matching,” in Medical Image Computing and Computer Assisted Intervention − MICCAI 2017: 20th International Conference, Quebec City, QC, Canada, September 11-13, 2017, Proceedings, Part I, Springer International Publishing, 2017, pp. 266–274.
