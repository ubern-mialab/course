# Voxel-wise tissue Classification



### Why is this done?

Classification assigns labels to different regions or structures within the image based on the extracted features.&#x20;

### How is it done?

This step often involves machine learning algorithms such as:

* **Support Vector Machines (SVM)**: For binary or multi-class classification.
* **Random Forests**: For handling complex, high-dimensional data.
* **Deep Learning Models**: Such as Convolutional Neural Networks (CNNs) for more complex and accurate classification tasks.

Do other machine learning algorithms perform better on our task? Can we improve the segmentation performance by parameter tuning?

* Overfitting
* Parameter tuning (tree depth, forest size)
* Support Vector Machine (SVM)
* Variants of decision forests (e.g., gradient boosted trees)

### Coding Resources

`scikit-learn: Supervised learning <http://scikit-learn.org/stable/supervised_learning.html#supervised-learning>`\_



TODO: also list project ideas in this component.

### References

A. Criminisi and J. Shotton, Decision Forests for Computer Vision and Medical Image Analysis, 1st ed. London: Springer, 2013.

R. S. Olson, W. La Cava, Z. Mustahsan, A. Varik, and J. H. Moore, Data-driven Advice for Applying Machine Learning to Bioinformatics Problems, Aug. 2017.

###

### Deep Learning

Deep learning has gained much attention in the last years outperforming methods such as decision forests. What is the performance of a deep learning method on our task?

`Generic U-Net Tensorflow implementation for image segmentation <https://github.com/jakeret/tf_unet>`\_

`U-Net PyTorch implementation for brain MRI <https://pytorch.org/hub/mateuszbuda_brain-segmentation-pytorch_unet/>`\_

O. Ronneberger, P. Fischer, and T. Brox, U-Net: Convolutional Networks for Biomedical Image Segmentation, May 2015.
