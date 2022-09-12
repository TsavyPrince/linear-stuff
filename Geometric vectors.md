Dependencies | Dependents
------------ | ------------
[[Abstract vectors]] | [[Span and basis]], [[Vector products]] 

So you might've been told that vectors are quantities with magnitude and direction, which can be represented by arrows, and yeah those are vectors but only a specific kind called Euclidean or **geometric vectors**. This is also why I named the last page *Abstract vectors*.

From now on, we'll almost exclusively be using geometric vectors, but the majority of concepts still work on general **abstract vectors**.

Geometric vectors can be notated as columns of real numbers. We call these real numbers **components** and notate the $i$th component of a vector $\mathbf{v}$ as a superscript like $\mathbf{v}^i$:
$$\begin{bmatrix}\mathbf{v}^1\\\mathbf{v}^2\\\mathbf{v}^3\\\vdots\\\mathbf{v}^n\end{bmatrix}$$
Occasionally, we may also notate components using subscripts like $\mathbf{v}_i$ (Actually, whenever we use a subscript, its not quite a geometric vector component but it doesn't matter for now). Superscripts and subscripts come up a lot and we call them **indices**.

Thankfully, using superscripts as indices almost never comes into conflict with exponents because exponents are so rare in linear algebra to begin with.

Adding two geometric vectors is simply adding their corresponding components:
$$\begin{bmatrix}\mathbf{u}^1\\\mathbf{u}^2\\\mathbf{u}^3\\\vdots\\\mathbf{u}^n\end{bmatrix}+\begin{bmatrix}\mathbf{v}^1\\\mathbf{v}^2\\\mathbf{v}^3\\\vdots\\\mathbf{v}^n\end{bmatrix}=\begin{bmatrix}\mathbf{u}^1+\mathbf{v}^1\\\mathbf{u}^2+\mathbf{v}^2\\\mathbf{u}^3+\mathbf{v}^3\\\vdots\\\mathbf{u}^n+\mathbf{v}^n\end{bmatrix}$$Scaling a geometric vector is simply multiplying its components:
$$a\begin{bmatrix}\mathbf{v}^1\\\mathbf{v}^2\\\mathbf{v}^3\\\vdots\\\mathbf{v}^n\end{bmatrix}=\begin{bmatrix}a\mathbf{v}^1\\a\mathbf{v}^2\\a\mathbf{v}^3\\\vdots\\a\mathbf{v}^n\end{bmatrix}$$

We identify special vectors, called **standard basis vectors**, which are notated as $\mathbf{e}_i$, which are $0$ everywhere except for their $i$th index, which is $1$. More succinctly $(\mathbf{e}_i)^j=\delta_i^j$ where $\delta$ is the **Kronecker delta**. $\delta^i_j=1$ when $i=j$ and $\delta^i_j=0$ anytime else. This sort of behavior comes up enough that we have to have a dedicated symbol for it. We usually write it with one upstairs index and one downstairs index, but occasionally we might have to have two downstairs or two upstairs indices.

Then every vector satisfies the following property:
$$\mathbf{v}=\sum_i\mathbf{v}^i\mathbf{e}_i$$
As it turns out, whenever we have an index which appears twice in a single term, once as a subscript, once as a superscript, it is almost always a sum so we can simply omit the summation sign:
$$\mathbf{v}=\mathbf{v}^i\mathbf{e}_i$$
This is called Einstein notation and is especially convenient later on when we'll deal with a ton of indices. From here on out, I'll probably be exclusively using Einstein notation.

We can rewrite the rules for addition and scaling as follows:
$$\mathbf{u}+\mathbf{v}=\mathbf{u}^i\mathbf{e}_i+\mathbf{v}^i\mathbf{e}_i$$
$$a\mathbf{v}=a\mathbf{v}^i\mathbf{e}_i$$
The components can act as coordinates in space, which lends itself to the visualization of vectors as arrows, with their tail at the origin, and their head at the point whose coordinates are the components of the vector. Then vector addition and scaling can be represented geometrically as follows:

![[vectoraddition.png\|128]] | ![[vectorscaling.png\|128]]
------------ | ------------

#linear_algebra