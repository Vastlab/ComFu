# ComFu
ComFu: Improving Visual Clustering by Commonality Fusion

# Abstract
ComFu presents a new formalization of clustering fusion and introduces the novel Commonality Fusion (ComFu) technique to combine the advantages of different clustering algorithms by fusing their results on datasets.
ComFu builds a pairwise commonality matrix of samples by computing how many clustering algorithms group each pair together.
Using this matrix, ComFu builds initial clusters of points with high commonality and then assigns points with low commonality to clusters with the highest average commonality to those points with an automatic distance measure selection process.
We start experiments by comparing ComFu with the prior state-of-the-art cluster fusion algorithms on eight UCI datasets.
We then evaluate ComFu on practical vision clustering problems, advancing the state-of-the-art on a wide range of applications including clustering faces in the IJB-B dataset.
We apply ComFu to fuse FINCH, the state-of-the-art "parameter-free" approach, which returns multiple partitions and can use multiple distance metrics, and show that ComFu improves their result by fusing over metrics and partitions.
