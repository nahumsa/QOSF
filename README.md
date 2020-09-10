# QOSF

QSOF Mentorship Task


# Task Selected: 4

Find the lowest eigenvalue of the following matrix:

[1 0 0 0; 

0 0 -1 0;

0 -1 0 0; 

0 0 0 1]

using VQE-like circuits, created by yourself from scratch.

In general, this exercise might be pretty difficult, so below there are a couple of tips. We’ve written them in a pale font so that those of you who embrace the challenge don’t look at them accidentally ;) 
PLEASE DON’T CHANGE THE COLOR OF THE FOLLOWING PARAGRAPH!
OTHER PEOPLE SEE THE CHANGES – IF YOU WANT TO READ WHAT’S THERE, JUST COPY IT ELSEWHERE.


It requires decomposing the matrix to the sum of Pauli terms. 
Decomposition involves only terms consisting of the same matrices, i.e.: II, XX, YY, ZZ, and the coefficients are from the set [-1/2, -1, 0, 1, 1/2].
The ansatz you can use is: (RX I) CX (HI) |00>, where angle in RX is your variational parameter.
You can find an explanation of VQE in this blog post, You can also find links to further resources there.
You can just search through all angles for RX, you don’t need to use any optimizers like gradient descent.
