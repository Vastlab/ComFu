# ComFu
ComFu: Improving Visual Clustering by Commonality Fusion

# Abstract
ComFu presents a new formalization of clustering fusion and introduces the novel Commonality Fusion (ComFu) technique to combine the advantages of different clustering algorithms by fusing their results on datasets.
ComFu builds a pairwise commonality matrix of samples by computing how many clustering algorithms group each pair together.
Using this matrix, ComFu builds initial clusters of points with high commonality and then assigns points with low commonality to clusters with the highest average commonality to those points with an automatic distance measure selection process.
We start experiments by comparing ComFu with the prior state-of-the-art cluster fusion algorithms on eight UCI datasets.
We then evaluate ComFu on practical vision clustering problems, advancing the state-of-the-art on a wide range of applications including clustering faces in the IJB-B dataset.
We apply ComFu to fuse FINCH, the state-of-the-art "parameter-free" approach, which returns multiple partitions and can use multiple distance metrics, and show that ComFu improves their result by fusing over metrics and partitions.

# System Overview
[ComFu_teaser.pdf](https://github.com/Vastlab/ComFu/files/10196395/ComFu_teaser.pdf)

![ComFu_teaser](https://user-images.githubusercontent.com/20711687/206746475-c2e053f9-f4e6-45e0-baea-e459d64b7622.jpg)

ComFu improves clustering by fusing different clustering results balancing the goal of commonality with noise reduction.
Given different base clustering results, we compute a commonality matrix by counting how often each pair of points in the dataset co-occur in the same cluster. 
We first build initial clusters from reliable pairs with high commonality and then assign the remaining points to maximize their commonality with existing clusters.
