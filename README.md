# k-means
I'll start with a brief explanation of what the K-Means algorithm does.
When analyzing data, one way to identify patterns is through clustering, which groups similar data points. The K-Means algorithm does this by using centroids—k randomly placed points that serve as the initial centers of the clusters.
First, we calculate the distance between each data point and the centroids, assigning each point to its closest centroid. This is the clustering step.
After the first iteration, we update the centroids by computing the mean (average) position of all the points in each cluster. These new centroids replace the old ones, and the process repeats.
Over multiple iterations, the centroids gradually stabilize, meaning their positions no longer change significantly. At this point, the algorithm converges, and clustering is complete.
However, some challenges arise with this approach:
Choosing the optimal number of centroids (k)—how do we determine the best value for k?


Random initialization—how do we ensure that the initial centroids lead to the most optimized clustering instead of a poor local minimum?


In this project, I'll address these issues and explore potential solutions.
Finally, I'll parallelize the code to improve efficiency.

Hardware and software.
My computer is an MSI GF63 Thin 10SC, running Windows 11 Home 64-bit, with the Intel Core i5-9300H processor, featuring 4 cores and 8 threads, and a base clock of 2.4 GHz (boost up to 4.1 GHz). It is equipped with 8GB of RAM and an NVIDIA GTX 1650 GPU, making it suitable for computational workloads. Additionally, the system is running BIOS version E16R5IMS.103 (released on May 14, 2021) and includes EC version 16R5EMS1.1020311202117:10:24.

My development environment includes Visual Studio Code as my primary code editor and OpenMP for C++ to leverage multi-core processing.
