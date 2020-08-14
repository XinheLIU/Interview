# Linear Algebra

### Concepts

##### Vectors and Matrix

* vectors
* linear system and matrix
  * geometric - linear combination
  * operation/transformation
* matrix operations
* invertible and singular matrix
  * [permutation matrix](https://en.wikipedia.org/wiki/Permutation_matrix)
* Gaussian elimination
  * Echelon matrix
  * pivot variables, \(\# = C\(A\)\), free variable\(\# = N\(A\)\)
  * [elementary matrix](https://en.wikipedia.org/wiki/Elementary_matrix)
* Null matrix
* matrix factorization
  * [LU Decomposition](https://en.wikipedia.org/wiki/LU_decomposition)

##### Vector Space

* vector space - definition
  * commutative, associative, distributive, unique identity
  * uniqueness of identity and inverse
* subspace
  * row space C\(A^T\)
    * pivot rows
  * column space C\(A\)
    * **Ax = b** &lt;=&gt; b in C\(A\)
  * null space N\(A\)/kernel
    * **Ax = 0**
  * Solution of Linear System 
    * pivot variables, free variables
    * Null space matrix
    * special solution 
    * left null space N\(A^T\)
  * m x n matrix by rank r
    * r = m = n : square and invertible
    * r = m &lt; n : short and wide: infinity number of solutions
    * r = n &lt; m : Tall and thin, 0 or 1 solution
    * r &lt; m, n : Not full rank, 0 or infinity solutions
  * rank
    * number of pivot column = dim C\(A\)
    * freedom = \# of free columns = dim N\(A\)
* span
  * Linearly independent
* basis
  * **basis of matrix spaces and function spaces**
* dimension
* orthogonality
  * **Fundamental Theorem of Linear Algebra**
    * orthogonal subspaces 
      * row space and null space
      * column space and left null space
  * projection
    * projection to vector - [projection matrix](https://mathworld.wolfram.com/ProjectionMatrix.html) \($$\frac{\mathbf{aa^T}}{\mathbf{a^Ta}}$$\)
    * projection to subspace
      * orthogonal to C\(A\) - A^T\(b-Ax\) = 0
      * [hat matrix/projection matrix ](https://en.wikipedia.org/wiki/Projection_matrix): A\(A^TA\)^-1A^T
  * Gram-Schmidt Process
    * orthonormal
    * orthogonal matrix Q
  * **QR Decomposition**
  * Matrix Space, function space
    * rank 1 matrix

##### Determinant

* basic properties
  * I -&gt; 1
  * exchange rows -&gt; reverse sign
  * linear in row 1\(i\) by itself
  * two rows equal, its determinant is 0
  * t times row i add to row j does not change
  * row of all zeros -&gt; 0
  * triangular matrix determinant -&gt; product of diagonal
  * A is **singular** then det A = 0
  * det BA = \(det B\) \* det\(A\)
  * det \(A^T\) = det A
* calculation
  * big formula
  * cofactors formula
* Cramer's rule 
* Cross product, outter product/Volume

##### Eigen Value & Eigen Vector

* transform invariability 
* properties
  * linearity - add
  * multiply - P^k, lambda ^ k
  * sum = trace, product \(=det\(A\)\) \(= product of pivots\)
  * det\(A-\lambda I\)
  * complex eigen value
  * commuting matrices share eigen values
* Eigen Space
  * geometric multiplicity
  * algebraic multiplicity
* Differential equations
  * linear differential equation system
* Markov matrices
* Fourier Series

##### Diagonalization

* Diagonalizable matrix
  * eigen space dimension = number of independent eigen vectors \(geometirc multiplicity\)
  * repetitions of eigen values = n roots of $$det(A - \lambda I ) = 0$$ \(characteristic polynomial\)
* Real matrix
  * eigen value and vector comes in conjugate pairs
* Real Symmetric matrix
  * [Spectral Theorem](https://en.wikipedia.org/wiki/Spectral_theorem) 
    * real eigen values \(all diagonailzable\)
    * eigen vectors can be chosen orthonormal \($$Q\Lambda Q^T$$\)
  * [Cholesky Decomposition](#)
* Positive definite matrices
  * x^T A x &gt; 0
    * positive eigen values 
    * pivots positive
    * principal submatrices positive definite
    * det\(A\) = 0 \(invertible\)
  * Cholesky R^T R with independent columns
* Positive semidefinite Matrices
  * **0 eigen value, depedent columns**
  * unit square root -&gt; Cholesky
* Similarity
  * B = M^-1 A M
  * **same eigen value, trace, determinant, rank, eigen space dimenstion, **
  * different Null, column space, **eigen vectors**, sigular values
  * [**Jordan Form**](https://en.wikipedia.org/wiki/Jordan_normal_form), Jordan Block
    * Generalized Eigenvector

##### Singular Value Decomposition

* $$A = U \Sigma V^T = \sum \mathbf{u_i} \sigma_i \mathbf{v_i^T}$$
  * $$AV = U \Sigma$$
* basis
  * V: first r from row space \(eigen values of A^TA\), n - r from null space
  * U: r from column space\(eigenvalues of AA^T\), n - r from left null space
* singular vectors
* in case of positive semidefinite\(orthonormal eigen vector, non negative eigen value\), same as eigen decomposition

##### Linear Transformation

* range: column space
* kernel: null space
* linearity based on basis - represent by matrix
  * eg. projection, integral, derivative, rotation
  * Wavelet transform
  * Discrete Fourier Transform
    * Fourier Matrix
    * Fast Fourier

##### Complex Matrices

* Hermitian
* Inner product in complex space



### Questions

* Solve a linear equation
* relationship between Ax=b and Ax = 0
  * special solution, rank, and linear space
* when is a matrix invertible \(A-1b as only solution\)
* full row rank vs full column rank
  * full column rank
    * all columns are pivot columns
    * no free variables \(null space 0 dimension\)
    * invertible, determined
  * full row rank 
    * columns spans whole space
    * n - r = n - m solutions
    * if m &lt; n, undetermined



