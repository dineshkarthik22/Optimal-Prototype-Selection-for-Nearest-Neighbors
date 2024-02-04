# Optimal-Prototype-Selection-for-Nearest-Neighbors
Discusses few prototype selection algorithms for Nearest Neighbor Algorithm

## Abstract
This study explores the significance of prototype selection techniques in enhancing the efficiency and effectiveness of the K-Nearest Neighbors algorithm for classification tasks. Prototype selection aims to reduce the dataset's size while preserving its representativeness, thereby mitigating the computational complexity associated with KNN. The study investigates three prototype selection methods: Random selection, K-Means clustering, and Modified Condensed Nearest Neighbor (MCNN). Through empirical experiments on the MNIST dataset, evaluated the impact of varying the number of prototypes (M) on the algorithm's accuracy, Balanced Error Rate (BER), and F1-Score. The results highlight the trade-offs between computational efficiency and classification performance.

## Description:
### Random Selection:
Random selection serves as the simplest approach, akin to blindly grabbing a handful of instances from the dataset. While lacking a strategic basis, this method provides a baseline for comparison, assessing how well KNN performs with an arbitrary subset.

### K-Means Clustering:
K-Means clustering takes a more structured approach by grouping similar instances together into clusters. The center of each cluster becomes a prototype, offering a condensed representation of the dataset.

### Modified Condensed Nearest Neighbor:
MCNN dynamically refines the prototype set during training, discarding instances that do not contribute significantly to the classification process. By selectively keeping instances crucial for decision boundaries, MCNN adapts to the dataset's complexity, potentially enhancing KNN's efficiency and accuracy.

## Experimental Results:
The experimental results present a comprehensive analysis of three different prototype selection strategies, namely random selection, k-means clustering, and Modified Condensed Nearest Neighbor (MCNN), applied to the MNIST classification task. The primary focus is on evaluating their classification performance and execution time across various prototype subset sizes. Both \textbf{MCNN and K-Means consistently demonstrates competitive accuracy, especially as M increases}. This indicates that both the  strategies are effective in selecting prototypes that generalize well to the entire dataset.

K-Means also illustrate high efficiency in terms of classification accuracy as it aims to partition the data into distinct clusters by \textbf{minimizing the sum of squared distances between data points and their assigned cluster centers}. By subsequently selecting prototype points based on these cluster centers, K-means effectively captures the inherent structure and distribution of the data. The elevated execution time observed for MCNN and K-means compared to the random strategy can be attributed to the \textbf{additional computational overhead involved in the iterative processes} of these selection methods.

## Conclusion:
In conclusion, the study made for selecting prototype models for K-Nearest Neighbor algorithm, illustrates that not only the prototype selection increases the accuracy of KNN on test set but also increases the runtime of the entire model. The trade-off between accuracy and efficiency is inevitable but considering better data structures and reducing the algorithmic complexity, the trade-off can be reduced to a particular extent.
