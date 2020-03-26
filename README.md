### NMF Algorithm
Non-negative Matrix Factorisation (NMF): Family of linear algebra
algorithms for identifying the latent structure in data represented
as a non-negative matrix.
<br>
<img src="notebook_images/nmf.png">
<br>
<pr>Input: matrix A; rank k.<br>
Output: Two k-dimensional factors W and H approximating A</pr><br>
<b>So our Objective function looks like this :</b>
<br>


<img src="notebook_images/nmf2.png">
<br>
<br>
<br>
<pr>There are several approaches inorder to solve this minimization Problem. 
I used <b>Multiplicative Update Method</b> <br>introduced by Lee and Seung in 1999. (<a href="https://papers.nips.cc/paper/1861-algorithms-for-non-negative-matrix-factorization.pdf">This Paper</a>)</pr>

### NNDSVD Method
As the <b>Multiplicative Update</b> is an iterative method, It is very senstive to initializations of W and H. <br>
<b>NNDSVD Method</b> is a SVD based initialization, introduced by C. Boutsidis and E. Gallopoulos in 2007 (<a href="http://scgroup.hpclab.ceid.upatras.gr/faculty/stratis/Papers/HPCLAB020107.pdf">This Paper</a>)
