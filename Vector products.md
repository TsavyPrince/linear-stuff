Dependencies | Dependents
------------ | ------------
[[Geometric vectors]] | [[Matrices]], [[The exterior product]], [[Covectors]]

You might've noticed we have failed to mention any product between vectors of any sort. That is not only because they are not essential for a vector space, but there are several different types.

The first one is the **dot product** or inner product or scalar product. To compute the dot product of two vectors, $\mathbf{u}\cdot\mathbf{v}$, you simply multiply the corresponding components together and sum all of them:
$$\mathbf{u}\cdot\mathbf{v}=\mathbf{u}^i\mathbf{v}_i$$
The dot product satisfies the following identity:
$$\mathbf{u}\cdot\mathbf{v}=|\mathbf{u}||\mathbf{v}|\cos(\theta)$$
where the length of a vector $\mathbf{v}$ is notated by $|\mathbf{v}|$ and $\theta$ is the angle between $\mathbf{u}$ and $\mathbf{v}$. This identity implies that the dot product of two vectors is always zero when the vectors are perpendicular.

In fact $|\mathbf{v}|$ is simply $\sqrt{\mathbf{v}\cdot\mathbf{v}}$. We can illustrate this fact using this equation and the Pythagorean theorem:
$$\begin{bmatrix}\mathbf{v}^1\\\mathbf{v}^2\end{bmatrix}\cdot\begin{bmatrix}\mathbf{v}^1\\\mathbf{v}^2\end{bmatrix}={(\mathbf{v}^1)}^2+{(\mathbf{v}^2)}^2$$

The second one is the **cross product** or vector product of three-dimensional vectors $\mathbf{u}\times\mathbf{v}$:
$$\mathbf{u}\times\mathbf{v}={\varepsilon^i}_{jk}u^jv^k\mathbf{e}_i$$
${\varepsilon^i}_{jk}$ is the **Levi-Civita symbol** $\varepsilon_{ijk}$ but with one of its indices raised. $\varepsilon_{ijk}$ is $0$ if any of the indices are equal, $1$ if $(i,j,k)$ is a result of an even amount of swapping of elements in $(1,2,3)$, and $-1$ for an odd amount of swapping.

This definition is not all that useful, so here is a more useful one:
$$\mathbf{u}\times\mathbf{v}=\mathbf{e}_1(\mathbf{u}_2\mathbf{v}_3-\mathbf{u}_3\mathbf{v}_2)+\mathbf{e}_2(\mathbf{u}_3\mathbf{v}_1-\mathbf{u}_1\mathbf{v}_3)+\mathbf{e}_3(\mathbf{u}_1\mathbf{v}_2-\mathbf{u}_2\mathbf{v}_1)$$
This still doesn't give much intuition. However, one can think of the cross product $\mathbf{u}\times\mathbf{v}$ as the vector, whose area is the parallelogram formed by using $\mathbf{u}$ and $\mathbf{v}$ as edges, perpendicular to both $\mathbf{u}$ and $\mathbf{v}$ whose direction is that which your right hand's thumb would point if your right hand's index finger was $\mathbf{u}$ and your middle finger was $\mathbf{v}$. This is called the right hand rule for obvious reasons.

It satisfies a trigonometric identity, similar to the one for the dot product:
$$\mathbf{u}\times\mathbf{v}=|\mathbf{u}||\mathbf{v}|\sin(\theta)\mathbf{n}$$
where $\mathbf{n}$ is a vector of length $1$ perpendicular to both $\mathbf{u}$ and $\mathbf{v}$ whose direction is dependent on the right hand rule. This identity implies that the dot product of two vectors is always zero when the vectors are aligned.

All of these formulas still suck but these identities are sufficient to derive the cross product of any two vectors:
* $\mathbf{e}_2\times\mathbf{e}_3=\mathbf{e}_1$
* $\mathbf{e}_3\times\mathbf{e}_1=\mathbf{e}_2$
* $\mathbf{e}_1\times\mathbf{e}_2=\mathbf{e}_3$
* Anticommutativity of the cross product: $\mathbf{u}\times\mathbf{v}=-(\mathbf{v}\times\mathbf{u})$
* Compatibility of the cross product with scaling: $a(\mathbf{v}\times\mathbf{w})=(a\mathbf{v})\times\mathbf{w}+\mathbf{v}\times(a\mathbf{w})$
* Right distributivity of the cross product over vector addition: $\mathbf{u}\times(\mathbf{v}+\mathbf{w})=\mathbf{u}\times\mathbf{v}+\mathbf{u}\times\mathbf{w}$
* Left distributivity of the cross product over vector addition: $(\mathbf{u}+\mathbf{v})\times\mathbf{w}=\mathbf{u}\times\mathbf{w}+\mathbf{v}\times\mathbf{w}$

Then we can derive this formula:
$$\begin{aligned}\mathbf {u} \times \mathbf {v} ={}&\quad \ \mathbf{u}^{1}\mathbf{v}^{1}\mathbf {0} +\mathbf{u}^{1}\mathbf{v}^{2}\mathbf{e}_3 -\mathbf{u}^{1}\mathbf{v}^{3}\mathbf{e}_2 \\&-\mathbf{u}^{2}\mathbf{v}^{1}\mathbf{e}_3 +\mathbf{u}^{2}\mathbf{v}^{2}\mathbf {0} +\mathbf{u}^{2}\mathbf{v}^{3}\mathbf{e}_1 \\&+\mathbf{u}^{3}\mathbf{v}^{1}\mathbf{e}_2 \ -\mathbf{u}^{3}\mathbf{v}^{2}\mathbf{e}_1 \ +\mathbf{u}^{3}\mathbf{v}^{3}\mathbf {0}\end{aligned}$$
Note that the cross product is not associative:
$$\left(\begin{bmatrix}1\\0\\0\end{bmatrix}\times\begin{bmatrix}1\\1\\0\end{bmatrix}\right)\times\begin{bmatrix}1\\1\\1\end{bmatrix}=\begin{bmatrix}-1\\1\\0\end{bmatrix}$$
$$\begin{bmatrix}1\\0\\0\end{bmatrix}\times\left(\begin{bmatrix}1\\1\\0\end{bmatrix}\times\begin{bmatrix}1\\1\\1\end{bmatrix}\right)=\begin{bmatrix}0\\0\\-1\end{bmatrix}$$

While we're at it, let's list most of the important identities which the dot product and cross product satisfy in one list:
* Commutativity of the dot product: $\mathbf{u}\cdot\mathbf{v}=\mathbf{v}\cdot\mathbf{u}$
* Compatibility of the dot product over scaling: $a(\mathbf{u}\cdot\mathbf{v})=(a\mathbf{u})\cdot\mathbf{v}$
* Distributivity of the dot product over vector addition: $\mathbf{u}\cdot(\mathbf{v}+\mathbf{w})=\mathbf{u}\cdot\mathbf{v}+\mathbf{u}\cdot\mathbf{w}$
* Anticommutativity of the cross product: $\mathbf{u}\times\mathbf{v}=-(\mathbf{v}\times\mathbf{u})$
* Compatibility of the cross product with scaling: $a(\mathbf{v}\times\mathbf{w})=(a\mathbf{v})\times\mathbf{w}+\mathbf{v}\times(a\mathbf{w})$
* Jacobi identity: $\mathbf{u}\times(\mathbf{v}\times\mathbf{w})+\mathbf{v}\times(\mathbf{w}\times\mathbf{u})+\mathbf{w}\times(\mathbf{u}\times\mathbf{v})=\mathbf{0}$
* Right distributivity of the cross product over vector addition: $\mathbf{u}\times(\mathbf{v}+\mathbf{w})=\mathbf{u}\times\mathbf{v}+\mathbf{u}\times\mathbf{w}$
* Left distributivity of the cross product over vector addition: $(\mathbf{u}+\mathbf{v})\times\mathbf{w}=\mathbf{u}\times\mathbf{w}+\mathbf{v}\times\mathbf{w}$


#linear_algebra