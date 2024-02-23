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
