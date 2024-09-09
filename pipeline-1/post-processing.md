# Post-processing



### Why is this done?



### How is it done?

Can we leverage the segmentation performance by post-processing?

* Morphological operators
* Dense conditional random field (CRF)
* Manual user interaction (e.g., brushing)

### Coding Resources

* `mialab.filtering.postprocessing`, e.g. use `DenseCRF`

TODO: also list project ideas in this component.

### References

P. Krähenbühl and V. Koltun, Efficient Inference in Fully Connected CRFs with Gaussian Edge Potentials, Advances in Neural Information Processing Systems, vol. 24, pp. 109-117, 2011.

S. Nowozin and C. H. Lampert, Structured Learning and Prediction in Computer Vision, Foundations and Trends in Computer Graphics and Vision, vol. 6, pp. 185-365, 2010.

P. Cattin, Image Segmentation, 2016. \[Online]. Available: https://www.miac.unibas.ch/SIP/pdf/SIP-07-Segmentation.pdf \[Accessed: 08-Sep-2020], see chapter 6 - Mathematical Morphology
