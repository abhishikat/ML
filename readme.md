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
