# EvoSplit

**EvoSplit** presents a new approach for the distribution of multi-label data sets into disjoint subsets for supervised machine learning. Currently, data set providers either divide a data set randomly or using iterative stratification [[1]](#1) [[2]](#2), a method that tries to maintain the labels (or label pairs) distribution of the original data set into the different subsets. Following this objective, EvoSplit offers two evolutionary approaches: First, a single-objective evolutionary algorith that aims at obtaining a split that maximises the similarity between those distributions independently. Second, a new multi-objective evolutionary algorithm to maximise the similarity considering simultaneously both distributions (labels and label pairs). **EvoSplit** improves the splitting of a data set in comparison to the iterative stratification.

## Code

I will make available the code soon here.

## New train/test splits of datasets available with [scikit-multilearn](http://scikit.ml/)

The new splits are available [here](https://drive.google.com/drive/folders/161X_IV4AamqK2nrHGcCvkvRc6dLlpfk8?usp=sharing). They can be uploaded using [skmultilearn.dataset.load_dataset_dump()](http://scikit.ml/api/skmultilearn.dataset.html). Similarly to [skmultilearn](http://scikit.ml/datasets.html), train, test, and undivided variants are provided. 

## New train/validation/test splits of well-known multi-label datasets

* Microsoft COCO - Panoptic Segmentation Task: [New splits](https://drive.google.com/drive/folders/1MzD2JbFWKe0jHSQJtMYxDf-kUgURrr3r?usp=sharing). The original data set can be downloaded from the [Microsoft COCO dataset website](https://cocodataset.org/#download).
* Tencent ML-Images: I offer [new splits](https://drive.google.com/drive/folders/1GsEbwfQmVEIKKF06QiFWggCnm9Elef3i?usp=sharing) for both the ImageNet and OpenImages subsets. The original dataset can be downloaded from the [Tencent ML-Images repository](https://github.com/Tencent/tencent-ml-images).

## Citation

If you use the new train/validation splits, please cite [this paper](https://www.mdpi.com/2076-3417/11/6/2823):

```
@Article{evoSplit,
AUTHOR = {Florez-Revuelta, Francisco},
TITLE = {EvoSplit: An Evolutionary Approach to Split a Multi-Label Data Set into Disjoint Subsets},
JOURNAL = {Applied Sciences},
VOLUME = {11},
YEAR = {2021},
NUMBER = {6},
ARTICLE-NUMBER = {2823},
URL = {https://www.mdpi.com/2076-3417/11/6/2823},
ISSN = {2076-3417},
DOI = {10.3390/app11062823}
}

```

## Contact

Feel free to contact me if you have any question:

[Francisco Florez-Revuelta](https://www.dtic.ua.es/~florez) (francisco.florez [at] ua.es)  
Department of Computing Technology  
University of Alicante  
Spain

## References

<a id="1">[1]</a> 
Sechidis, K., Tsoumakas, G., & Vlahavas, I. (2011, September). On the stratification of multi-label data. In Joint European Conference on Machine Learning and Knowledge Discovery in Databases (pp. 145-158). Springer, Berlin, Heidelberg.

<a id="2">[2]</a> 
Szymański, P., & Kajdanowicz, T. (2017). A network perspective on stratification of multi-label data. arXiv preprint arXiv:1704.08756.
