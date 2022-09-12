Dependencies | Dependents
------------ | ------------
[[Geometric vectors]] | [[Change of basis]]

Ok, so you're probably familiar with the standard basis vectors $\mathbf{e}_i$ and how you can just scale them and add them together to get any vector in the space. The standard basis is not the only set of vectors that can do this.

We say a vector is a **linear combination** of some set $S$ of vectors if it can be constructed by vector addition and scaling on the elements of $S$. The set of vectors which are a linear combination of vectors in $S$ is called the **span** of $S$.

A set of vectors $B$ is called a **basis** of the space $V$ if and only if all of the vectors in $B$ span $V$ and no vector in $B$ can be constructed as a linear combination of any of the other vectors $B$.

Given that vectors in $\mathbb{R}^n$ are uniquely specified by $n$ coordinates, any basis of $\mathbb{R}^n$ simply has $n$ elements.

This provides us a good definition for the dimensionality of a vector space, namely, the number of elements any basis of the vector space has.

#linear_algebra