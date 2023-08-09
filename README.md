## **Handwritten Digit Classification using Unsupervised Learning**

### **Introduction:**
In this project, I undertook a classification task on the Semeion Handwritten Digit dataset using three unsupervised learning algorithms: Latent Class Analysis (LCA), Mean Shift, and Normalized Cut. I've evaluated and visualized the performance of each model based on the Rand index.

### **Dataset:**
**Semeion Handwritten Digit**: A collection of handwritten digits from 0-9. Each image can be visualized as vectors in a 256-dimensional Euclidean space.

### **Methodologies:**

1. **Latent Class Analysis (LCA):**
   - **Definition**: LCA groups subjects from multivariate data into “latent classes” based on hidden patterns in the data.
   - **Implementation**: Modified the number of latent classes to see its effect on the clustering outcome.
   
2. **Mean Shift**:
   - **Definition**: A centroid-based algorithm that discovers "blobs" in a smooth density of samples by updating candidates for centroids to be the mean of the points within a region.
   - **Implementation**: Adjusted the bandwidth parameter to explore its influence on clustering quality.
   
3. **Normalized Cut**:
   - **Definition**: An algorithm that optimally clusters a graph by minimizing cuts but also considers the volume inside clusters to create balanced groupings.
   - **Implementation**: Varied the number of clusters to study its impact.

### **Evaluation Metrics:**

- **Rand Index**: Used to measure the similarity between the true data labels and the labels predicted by the clustering algorithm.
  \( R = \frac{2(a+b)}{n(n-1)} \)
  where n is the number of images in the dataset, a represents the number of pairs of images that represent the same digit and are clustered together, and b is the number of pairs of images that represent different digits and are placed in different clusters.

### **Results & Discussions**:
1. **LCA** displayed the highest Rand index, making it the best performing algorithm in this assignment.
2. **Normalized Cut** closely followed LCA in performance, indicating its reliability and potential as a clustering algorithm.
3. **Mean Shift** lagged behind the other two in terms of Rand index, but its centroid-based approach offers unique insights.

### **Conclusion**:
The performance of each algorithm varied, with LCA being the standout. However, Normalized Cut also proved to be a valuable method due to its interpretability and balance in clustering. Future work might involve utilizing a larger dataset for more robust clustering.
