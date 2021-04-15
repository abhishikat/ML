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
    G = {‘?’, ‘?’,’?’,’?’…}: Number of attributes
    Specific Hypothesis: Specifying features to learn machine (Specific feature)
    S= {‘pi’,’pi’,’pi’…}: Number of pi depends on number of attributes.
    Version Space: It is intermediate of general hypothesis and Specific hypothesis. It not only just written one hypothesis but a set of all possible hypothesis based on training data-set.
