Dependencies | Dependents
------------ | ------------
[[Vector products]] | [[Change of basis]], [[Eigenstuff]]

**Matrices** are linear transformations, that is, a given matrix $\mathbf{A}$ is function that takes vectors and gives vectors and must satisfy the following identities:
* $\mathbf{A}(a\mathbf{v})=a\mathbf{A}(\mathbf{v})$
* $\mathbf{A}(\mathbf{u}+\mathbf{v})=\mathbf{A}(\mathbf{u})+\mathbf{A}(\mathbf{v})$

We notate matrices using uppercase bold letters like $\mathbf{A}$. Additionally, we can omit the parentheses so $\mathbf{A}(\mathbf{v})$ would become $\mathbf{A}\mathbf{v}$.

The set of matrices sending vectors of a space $V$ to vectors of a space $W$ is notated as $\mathrm{Hom}(V,W)$.

Since all vectors are linear combinations of some set of basis vectors, we can uniquely specify a matrix by where it sends the standard basis vectors $\mathbf{e}_i$. For example, we can specify a matrix from vectors in $\mathbb{R}^2$ to vectors in $\mathbb{R}^2$ by saying it sends $\mathbf{e}_1$ to $\begin{bmatrix}2\\1\end{bmatrix}$ and $\mathbf{e}_2$ to $\begin{bmatrix}3\\4\end{bmatrix}$. Then we can notate a matrix by simply gluing together where it sends the standard basis vectors in the order suggested by the indices:
$$\begin{bmatrix}2&3\\1&2\end{bmatrix}$$
This suggests that we can give the matrix $\mathbf{A}$ indices as follows:
$$\begin{bmatrix}\mathbf{A}^{1}_{1}&\mathbf{A}^{1}_{2}&\mathbf{A}^{1}_{3}&\cdots&\mathbf{A}^{1}_{n}\\\mathbf{A}^{2}_{1}&\mathbf{A}^{2}_{2}&\mathbf{A}^{2}_{3}&\cdots&\mathbf{A}^{2}_{n}\\\mathbf{A}^{3}_{1}&\mathbf{A}^{3}_{2}&\mathbf{A}^{3}_{3}&\cdots&\mathbf{A}^{3}_{n}\\\vdots&\vdots&\vdots&\ddots&\vdots\\\mathbf{A}^{m}_{1}&\mathbf{A}^{m}_{2}&\mathbf{A}^{m}_{3}&\cdots&\mathbf{A}^{m}_{4}\end{bmatrix}$$
Then, we can call the matrix $\mathbf{A}$ an $n\times m$ matrix.

Then we can come up with a formula for applying a matrix to a vector:
$$\mathbf{A}\mathbf{v}=\mathbf{v}^i\mathbf{A}^j_i\mathbf{e}_j$$

In addition to applying a matrix to a vector, we can also multiply two matrices together, which is simply function composition so that $\mathbf{B}(\mathbf{A}\mathbf{v})=(\mathbf{B}\mathbf{A})\mathbf{v}$. Note that the rightmost matrices are applied first, since matrices are functions. Interestingly, matrix multiplication is not commutative, as demonstrated by these two equations:
$$\begin{bmatrix}0&1\\0&0\end{bmatrix}\begin{bmatrix}0&0\\1&0\end{bmatrix}=\begin{bmatrix}1&0\\0&0\end{bmatrix}$$
$$\begin{bmatrix}0&0\\1&0\end{bmatrix}\begin{bmatrix}0&1\\0&0\end{bmatrix}=\begin{bmatrix}0&0\\0&1\end{bmatrix}$$

We can also add matrices together by simply adding their corresponding indices, just like how we add vectors together, and scale matrices, by simply multiplying their indices by the scaling factor. As a matter of fact, matrices are abstract vectors, although without the extra structure of their multiplication and application on vectors, the space of $n\times m$ matrices is functionally identical to $\mathbb{R}^{nm}$. An $n\times n$ matrix is called a square matrix. We notate matrix addition and scaling just like ordinary vector addition and scaling.

Like ordinary geometric vectors, we can also specify standard basis matrices $\mathbf{E}^i_j$, which have all their indices equal to $0$, except for $(\mathbf{E}^i_j)^j_i$, which is $1$. Then every matrix $\mathbf{A}$ satisfies the following identity:
$$\mathbf{A}=\mathbf{A}^i_j\mathbf{E}^j_i$$
We then derive these formulas for matrix addition and scaling:
$$a\mathbf{A}=a\mathbf{A}^i_j\mathbf{E}^j_i$$
$$\mathbf{A}+\mathbf{B}=\mathbf{A}^i_j\mathbf{E}^j_i+\mathbf{B}^i_j\mathbf{E}^j_i$$
as well as this formula for matrix multiplication:
$$\mathbf{B}\mathbf{A}=\mathbf{A}^i_k\mathbf{B}^j_i\mathbf{E}^k_j$$

#linear_algebra 
#matrices
#unfinished