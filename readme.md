## Program 1: Find S Algorithm
### Introduction :
    Find-S algorithm is a basic concept learning algorithm in machine learning. Find-S algorithm finds the most specific hypothesis that fits all the positive      examples. We have to note here that the algorithm considers only those positive training example. Find-S algorithm starts with the most specific hypothesis and generalizes this hypothesis each time it fails to classify an observed positive training data. Hence, Find-S algorithm moves from the most specific hypothesis to the most general hypothesis.

### Important Representation :

    ? indicates that any value is acceptable for the attribute.
    specify a single required value ( e.g., Cold ) for the attribute.
    ϕindicates that no value is acceptable.
    The most general hypothesis is represented by: {?, ?, ?, ?, ?, ?}
    The most specific hypothesis is represented by : {ϕ, ϕ, ϕ, ϕ, ϕ, ϕ}
### Steps Involved In Find-S :

    Start with the most specific hypothesis.
    h = {ϕ, ϕ, ϕ, ϕ, ϕ, ϕ}
    Take the next example and if it is negative, then no changes occur to the hypothesis.
    If the example is positive and we find that our initial hypothesis is too specific then we update our current hypothesis to general condition.
    Keep repeating the above steps till all the training examples are complete.
    After we have completed all the training examples we will have the final hypothesis when can used to classify the new examples.
## Program 2: Candidate Elimination Algorithm
### Introduction :
       The candidate elimination algorithm incrementally builds the version space given a hypothesis space H and a set E of examples. The examples are added one by one; each example possibly shrinks the version space by removing the hypotheses that are inconsistent with the example. The candidate elimination algorithm does this by updating the general and specific boundary for each new example. 

### You can consider this as an extended form of Find-S algorithm.
    Consider both positive and negative examples.
    Actually, positive examples are used here as Find-S algorithm (Basically they are generalizing from the specification).
    While the negative example is specified from generalize form.
### Terms Used:  

    Concept learning: Concept learning is basically learning task of the machine (Learn by Train data)
    General Hypothesis: Not Specifying features to learn the machine.
## Program 3: ID3 Algorithm
    ID3 stands for Iterative Dichotomiser 3 and is named such because the algorithm iteratively (repeatedly) dichotomizes(divides) features into two or more groups at each step.
    It, uses a top-down greedy approach to build a decision tree.
    In simple words, the top-down approach means that we start building the tree from the top and the greedy approach means that at each iteration we select the              best feature at the present moment to create a node.
    Most generally ID3 is only used for classification problems with nominal features only.

### ID3 Steps
    Calculate the Information Gain of each feature.
    Considering that all rows don’t belong to the same class, split the dataset S into subsets using the feature for which the Information Gain is maximum.
    Make a decision tree node using the feature with the maximum Information gain.
    If all rows belong to the same class, make the current node as a leaf node with the class as its label.
    Repeat for the remaining features until we run out of all features, or the decision tree has all leaf nodes.

## Program 4: Naive Bayes Classifier 
   ### What is a classifier?
        A classifier is a machine learning model that is used to discriminate different objects based on certain features.
   ### Principle of Naive Bayes Classifier:
        A Naive Bayes classifier is a probabilistic machine learning model that’s used for classification task.
        The crux of the classifier is based on the Bayes theorem.
   ### Bayes Theorem:

    Using Bayes theorem, we can find the probability of A happening, given that B has occurred. Here, B is the evidence and A is the hypothesis. 
    The assumption made here is that the predictors/features are independent. That is presence of one particular feature does not affect the other. 
    Hence it is called naive.
        G = {‘?’, ‘?’,’?’,’?’…}: Number of attributes
        Specific Hypothesis: Specifying features to learn machine (Specific feature)
        S= {‘pi’,’pi’,’pi’…}: Number of pi depends on number of attributes.
        Version Space: It is intermediate of general hypothesis and Specific hypothesis.
        It not only just written one hypothesis but a set of all possible hypothesis based on training data-set.
