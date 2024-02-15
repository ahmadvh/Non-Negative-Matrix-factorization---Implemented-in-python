### NMF Algorithm
Non-negative Matrix Factorization (NMF) is a family of linear algebra algorithms used for identifying the latent structure within data represented as a non-negative matrix.
[Link to the YouTube tutorial](https://youtu.be/o4pPTwsd-5M?si=dWtts9M32-VqurcX)

<br>
<img src="notebook_images/nmf.png">
<br>
<pr>Input: matrix A; rank k.<br>
Output: Two k-dimensional factors W and H approximating A</pr><br>
<b>So our Objective function looks like this:</b>
<br>

<img src="notebook_images/nmf2.png">
<br>
<br>
<pr>There are several approaches to solving this minimization Problem. 
I used <b>Multiplicative Update Method</b> <br>introduced by Lee and Seung in 1999. (<a href="https://www.researchgate.net/publication/2480786_Multiplicative_Updates_for_Nonnegative_Quadratic_Programming_in_Support_Vector_Machines">This Paper</a>)</pr>

### NNDSVD Method
As the <b>Multiplicative Update</b> is an iterative method, It is very sensitive to initializations of W and H. <br>
<b>NNDSVD Method</b> is an SVD-based initialization, introduced by C. Boutsidis and E. Gallopoulos in 2007 (<a href="https://www.sciencedirect.com/science/article/abs/pii/S0031320307004359">This Paper</a>)
