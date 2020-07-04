# svm-red-wine-quality

<p align="center">
  <img src="https://user-images.githubusercontent.com/47216809/86511259-ef33e380-be14-11ea-8ea3-3a3cc4ff5ce8.jpg">
</p>

<h1 align="center">
         WINE QUALITY ANALYSIS
</h1>

This mini project was made as a part of completion of the practical sessions in the subject Machine Learning. We have used a red wine quality dataset of the Portuguese "Vinho Verde" wine as the input to our program. These datasets can be viewed as classification or regression tasks. The classes are ordered and not balanced (e.g. there are much more normal wines than excellent or poor ones). Outlier detection algorithms could be used to detect the few excellent or poor wines. We train our model using the given 1599 instances of wine qualities and then use this trained model to predict the quality of wine using SVM from scratch.

<h2>
          Support Vector Machine:
</h2>
     In machine learning, support-vector machines (SVMs) are supervised learning models with associated learning algorithms that analyze data used for classification and regression analysis. Given a set of training examples, each marked as belonging to one or the other of two categories, an SVM training algorithm builds a model that assigns new examples to one category or the other, making it a non-probabilistic binary linear classifier (although methods such as Platt scaling exist to use SVM in a probabilistic classification setting). An SVM model is a representation of the examples as points in space, mapped so that the examples of the separate categories are divided by a clear gap that is as wide as possible. New examples are then mapped into that same space and predicted to belong to a category based on which side of the gap they fall.
     In addition to performing linear classification, SVMs can efficiently perform a non-linear classification using what is called the kernel trick, implicitly mapping their inputs into high-dimensional feature spaces.
For our dataset:
Suppose, we are taking two attributes from our dataset: free sulfur dioxide, total sulfur dioxide
From that we are classifying our dataset as good quality wine and bad quality wine using the two attributes.

Good quality wine = {[11, 28], [17, 21], [12, 18], [17, 31],…}
Bad quality wine = {[30, 35], [34, 30], [37, 44], [39, 34],…}

We would like to discover a simple SVM that accurately discriminates the two classes. Since the data is linearly separable, we can use a linear SVM (that is, one whose mapping function is the identity function). By inspection, it should be obvious that there are two support vectors;
S1 = {[17,31]}, S2 = {[30,35]}

The discriminating hyperplane corresponding to the values α1 =[17,51] ,α2 = [33,2], as we can visibly in the graph.

<p align="center">
  <img src="https://user-images.githubusercontent.com/47216809/86511378-248d0100-be16-11ea-8c9a-56ac56f64389.jpg">
</p>

In SVM, we have some hyperplane which separates the positive (yi = +1) from the negative (yi = -1) examples (a separating hyperplane). The points ‘x’ which lie on the hyperplane satisfy x ・ w + b = 0, where w is normal to the hyperplane. Here,    is the perpendicular distance from the hyperplane to the origin, and ||w|| is the Euclidean norm of w. Let d+(d-) be the shortest distance from the separating hyperplane to the closest positive (negative) example. The “margin” of a separating hyperplane is defined to be (d+) + (d-). For the linearly separable case, the support vector algorithm simply looks for the separating hyperplane with largest margin. 
This can be formulated as follows: suppose that all the training data satisfy the following constraints:  <p align="center">
  <img src="https://user-images.githubusercontent.com/47216809/86511411-83527a80-be16-11ea-9d7b-535560278fac.png">
</p>

Thus, the solution for a typical two dimensional case have the form shown in the above graph. Those training points for which the equality in constraint 1 holds (i.e. those which wind up lying on one of the hyperplanes H1, H2), and whose removal would change the solution found, are called support vectors; they are indicated in figure by the Red(‘<’) and Blue(‘>’) marks. 

<h2>
          Conclusion:
</h2>

Hence, we implemented SVM algorithm on red wine quality dataset which discriminates the two classes as good wine and bad wine quality respectively according to the physiochemical attributes of the red wine. We also built our own SVM from scratch which slightly gives more accuracy than the sklearn’s linear SVM.


\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\THANK - YOU///////////////////////////////////////////////////////////////////

          PROJECT CREATED BY - Prashant Wakchaure
          Email ID - prashant900555@gmail.com
          Contact No. - 8975366296
