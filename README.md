In this project, I implemented knn methods to apply classification problem according to service feature in our dataset. We had 4 service type in that feature. First, I read the data and visualized some features that I thought important. And I checked some values such as mean age, maximum salary etc. Then I encoded categorical variables to apply knn. I created train and test sets. Then I started to implement my knn methods. I used Euclidian Distance to measure distance. Then in find neighbor method, I iterated through training parameter and ordered distance list and find k neirest neighbors. Then I classified my points according to k neirest neighbors's classes.

For eliminated data part, I eliminated district,address,reside,gender,is_married,is_retired,customer_since features and applied my knn algorithm to that eliminated data. For scaled one, I scaled my data according to min max values and applied knn to that data.\n"

For weighted knns: I extended the basic knn algorithm by adding weights to the predictions. The weights were calculated inversely proportional to the distance between the test data and the neighbors in the training data. For class occurance weighted knn, the more frequent a class was the less weight it received, allowing the rarer classes to gain more importance. For combined weighted knn, I combined the weighted knn and occurance based weighted knn.

As seen from the result, weighted knns has more success in overall. To get higher accuracies, some improvements may be done:

Feature Engineering: Additional features (e.g., data normalization, feature enrichment) can be applied to the data.

Balancing the Dataset: If there is class imbalance in the training dataset, this can negatively affect the performance. Data augmentation techniques or balancing strategies can be applied to resolve this issue."
 Cross Validation may be useful.

My maximum k value was 19. Maybe higher k values may gets higher accuracies.
