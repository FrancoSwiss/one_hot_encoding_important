For a specific project, I can only Integer Encode, but not One-Hot Encode.

Many Machine Learning experts such as Sebastian Raschka ("Python Machine Learning") urge coders to do one-hot encoding. 
The main argument is that for categorical labels without an order, Integer Encoding can screw up your model. 
But there are also some disadvantages (introduction of correlation, overfitting...).

I did not want to look stupid in front of my customer, so I did what any reasonable ML coder does: 
I created my own dataset to test it.

SYNTHETIC DATASET:

50 sales people
A - H features (random variables ranging from 1-100)
20 examples (i.e each sales is represented 20 times).
1 sales person always with label 1.
The hypothesis is, that if I only Integer Encode each sales (sales 1 = 1, sales 2 = 2...), the model should struggle
because sales people are not ordinal (i.e. sales 40 is not better than sales 4).

RESULTS INCLUDED
