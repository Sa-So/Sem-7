# Descriptive Stats
- to summarize & describe datasets
- desc charecteristics of data
- if sample is normally distributed or not
- displayed through tables/charts/ freq. dist. and is gen. reported as a measure of central tendency.

## Central Tendency
1. Mean
2. Median
3. Mode

Mean and median can only be used for numerical data. 
The mode can be used with numerical and nominal data both.

## Statistical Dispersion
1. Range - gives us the understanding of how spread out the given data is
2. Variance - gives us the understanding of how the far the measurements are from
the mean.
3. Standard Deviation - √var - gives us the measurement of how far the data deviate from mean.

## Bell Curve
- Graph of normal dist. of a variable
1. Skewness - measure of asymmetry of a dist. of a variable about its mean.
2. Kurtosis - measure of "tailedness" of a dist. of a variable . It gives us understanding of how closely the data is spread out.

# Common char. used in desc. stats.
## Center 
- middle of data (3Ms are used as measures)
The disadvantage of using Mode is that there may be more than one mode.

## Spread 
- how data is dispersed 
- Range / IQR / Standard Deviation / Variance are the most commonly used as measures.
1. Range = Max – Min
2. Inter Quartile Range (IQR) = Q3 – Q1
3. Standard Deviation (σ) = √(∑(x-μ)2 / n)
4. Variance = σ2

## Shape
1. Symmetric – the part of the distribution that is on the left side of the median is same as the part of the distribution that is on the right side of the median
2. Left skewed – the left tail is longer than the right side
3. Right skewed – the right tail is longer than the left side

## Outlier 
– An outlier is an abnormal value
1. Keep the outlier based on judgement
2. Remove the outlier based on judgement

# Probability Distributions Inferential Statistics through hypothesis tests

In Inferential statistics, we make an inference from a sample about the population. The main aim of inferential statistics is to draw some conclusions from the sample and generalise them for the population data

## Advantages of Inferential Stats.
- Making conclusions from a sample about the population
- To conclude if a sample selected is statistically significant to the whole
population or not
- Comparing two models to find which one is more statistically significant as compared to the other.
- In feature selection, whether adding or removing a variable helps in improving the model or not.

## Probability
 It is a measure of the chance of occurrence of a phenomenon. We will now discuss some terms which are very important in probability:
* Random Experiment:Random experiment or statistical experiment is an experiment in which all the possible outcomes of the experiments are already known. The experiment can be repeated numerous times under identical or similar conditions.
* Sample space: Sample space of a random experiment is the collection or set of all the possible outcomes of a random experiment.
* Event: A subset of sample space is called an event.
* Trial: Trial refers to a special type of experiment in which we have two types
of possible outcomes: success or failure with varying Success probability.
* Random Variable: A variable whose value is subject to variations due to randomness is called a random variable. A random variable is of two types: Discrete and Continuous variable. In a mathematical way, we can say that a
real-valued function X: S -> R is called a random variable where S is probability space and R is a set of real numbers.

## Prob. Dist.
* A distribution is simply a collection of data or scores on a variable. Usually, these scores are arranged in order from ascending to descending and then they can be presented graphically.

* The distribution provides a parameterized mathematical function which will calculate the probability of any individual observation from the sample space.

*What is Data?*
* Data is a collection of information (numbers, words, measurements, observations) about
 facts, figures and statistics collected together for analysis. Example: Distribution
 individuals in each group. How to Visualize Categorical Data: Bar Plot, Pie Chart and Pareto Chart.

![*How to Visualize Numerical Data: Histogram, Line Plot and Scatter Plot*]()

---
### Variance 
- is the difference in fits between data sets.
### Bias 
- is the inability to capture the true relationship.

---
Squiggly line = overfit = large var = low bias
Straight line = underfit = low var = high bias

---
# SVMs
## Margin 
* shortest distance between observations and threshold.
    * maximal marginal classifier 
        * uses max margin i.e. divide the distance between 2 different classes observations !
        * not good if outliers ! (low bias but high var)
    * allow misclassifications - to make it unsensitive to outlier's
     * Bias - variance tradeoff pretty much
     * Now the distance between observations and threshold is called *Soft Margin*
     * We use Cross Validation to decide how many misclassifications (& correct classif. ) to allow (inside soft margin)!
     * It is called *Support Vector Classifier*
     * Observations on the edge and inside soft margin are called support vectors
     * when data is 2D SVC is a line ! (flat affine 1 D subspace)
     * when data is 3D SVC is a plane !(which side of plane are the point on)
     * 4D -> hyperplane (flat affine subspace)
     * 1D line = 1D hyperplane
     * SVC can handle overlapping classifications !
    * *SVM*
     * for data with too much overlap and eg. dosage and patients which got cured
     * they get cured when dosage is just right and not when high or low
     * We add a y axis with dosage^2 when x-axis has dosage and then do what we did in SVC
     1. start with data in low dimention
     2. Move data in higher dimention
     3. SVC!
     - SVM's use kernel functions to systematically find SVC in higher dimentions
     - Polynomial kernel has parameter d (degree of polynomial)
     - pk increases dimentians & d!
     - in 1D pk finds relationship b/w every pair of observations
     - Again we can find a good value of d using cross validation !
     - *Radial basis function Kernel* is also used , it finds SVC in ∞ dimensions
     - weighted nearest neighbour model ?
      - nearest neighbours have most influence 
     * **Kernel Trick** = calculating higher dimensional relationships between pairs of data without actual transformation to higher dimensions.
     * KT is the reason RDF is possible .
 





