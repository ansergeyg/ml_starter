When reading all these articles about Machine Learning in general and Neural Networks in pacticular you cannot help but notice that the way these NN models are build is mostly similar to one another.

THe genearal structure is pretty obvious.

First, you need to collect the data. Possiblly the most difficult and complicated step according to many authors I read. It requires parsing of raw data or manually processing data using some scripts.  

Then you need to prepare/preprocess data. This step looks more "standardized" than the first step of sheer parsing of raw data as it has "stable" techniques to properly process data to be fed to NN models.  

Finally, you can start to build a model using that data as input.

If we look at the models they kind of always use the same structure to write algorithms. You have input data then you set some layers and set some functions to process your input data and finally output some result.

The structure is always the same. You always use a certain set of mathematical functions to process some data built in layers. I never asked the question of WHY? Why it's always like that? The question was never conceptualized in my head until recently.

I found out in one of the articles that there is such thing as Universal Approximation Theorem. It is fundamental in the way that it basically says that:

a neural network with enough hidden neurons can approximate any continuous function on a compact set with any given accuracy.

Which basically means if all the criterias of this theorem are met then by trying proper different math functions and enough computing resources you can build pretty accureate model for absolutely anything (anything that can be represented as a valid input for your model)! 

That is why NN models mostly look the same. Because people just try to find proper functions to process their data more accurately. 


Links:

https://brilliant.org/wiki/newton-raphson-method/

---------------------------------------------------------------------------------------------

**Error/cost/loss function:**

Description goes here:

https://www.machinelearningworks.com/tutorials/mean-squared-error-cost-function

**Gradient descent**

Description goes here:

**Supervised and unsupervised learning**

In supervised learning you use labeled training data to train your model. Labeled data is prepared manually by people. The cost function then takes
labeled data (ideal expected parameters) and actual data (some input data) and is evaluated with respect to both expected and actual parameters. Now you can optimize (minimize/maximize)
the cost function using some optimization methods like gradient descent.

In unsupervised learning there is no labeled training data. Or is there any labeled data used in there?
It's kind of logical not to expected any human labeling in the unsupervised training as the name suggests however:

Labeled data has two distinct uses in ML:

1) Training
2) Validation

Unsupervised learning doesn't use training data (labeled data), but to actually find out if your algorithm works you still need some validation to comppare with.
In this way unsupervised learning does use labeled data but for validation.


**Good ml coding problems for exercising**

https://www.gptandchill.ai/codingproblems

----------------------------------------------------------------------------------------------
**Advaned stuff:**

https://www.tensorflow.org/text/tutorials/transformer
