# K-means
K-means(K 均值)算法是机器学习中常用的一种简单的聚类算法，该算法属于划分式聚类算法。其中，K 表示需要将数据集划分成的簇的个数。在运用Kmeans算法时，由于我们一般不知道数据的分布情况，也就无从得知数据的分簇的数目，所以一般通过枚举来确定 k 的值。另外，在实际应用中，由于K-means一般作为数据预处理，或者用于辅助分类贴标签，所以 k 值一般不会设置很大。
# 思想
K-means 算法的思想：首先，确定 k 个初始点作为分簇的中心；接着，将数据集中的每个点分配到一个簇中，即为每个点找到距离其最近的质心，并将其分配给该质心所对应的簇；然后，每个簇的中心更新为该簇所有点的平均值。再次重新分配数据集中所有的点，如果所有的点被分配的簇和之前一样，即簇的中心不会再改变，则此时的 k 个簇就是我们所需要的；如果某个点被分配的簇改变了，则分配完所有的点之后重新更新每个簇的质心，重复分配、更新操作直到所有簇的中心不再改变。
