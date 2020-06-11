# Introduction

### See the whitepaper in this repository for more description of the ideas.

### This notebook is experiments with a tree of centroids with an option to append them to the image.

### Experiments use one of two types of models for prediction: kNN and CNN. 

### kNN treats the 28x28 image as an array of 784 pixels and uses L2 distance metric. 

### CNN is lifted verbatim from the book "Deep Learning with Python" by Francois Chollet, 2018 (page 120-122) the inventor of Keras. The CNN is not SOTA but is useful to see whether adding information about centroids improve a neural net model.

### The training/testing set of images is either small (6,000/1,000) or large (60,000/10,000).

### The bottom line result is the error rate reduction.

## Results from experiments

| model\#images | 6,000 | 60,000 |
| --- | --- | --- |
| baseline kNN | 91.6% | 96.88% |
| improved kNN | 94.1% | 97.12% |

### and

| model\#images |  6,000  |  60,000  |
| --- | --- | --- |
| baseline CNN |  96.29%  |  99.02%  |
| improved CNN |  96.90%  |  99.10%  |

### From these results, the _*error rate reduction*_ is

| model\#images |  6,000  |  60,000  |
| --- | --- | --- |
| kNN |  29.76%  |  7.7%  | 
| CNN |  16.4%  |  9%  | 
