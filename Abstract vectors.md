Dependencies | Dependents
------------ | ------------
[[Linearity]] | [[Geometric vectors]]

Vectors are one of the most important concepts in linear algebra. They're objects which can be added together or scaled by some factor. However we have to define addition and scaling first, by defining vector spaces, of which a vector is an element of.

A **vector space** is a field $F$ along with a set $V$ which satisfies certain properties.

To start, we define what a field is. A **field** is a set $F$, equipped with two operations $+$ (**field addition**) and $\cdot$ (**field multiplication**) (we can omit the $\cdot$), of objects which satisfy the follow properties:
* Associativity of field addition: $(a+b)+c=a+(b+c)$
* Commutativity of field addition: $a+b=b+c$
* Identity of field addition: There exists an element $0$ of $F$ such that $a+0=a$
* Inverses of field addition: For every $a$ in $F$, there exists an element $-a$ of $F$ such that $a+(-a)=0$
* Associativity of field multiplication: $(ab)c=a(bc)$
* Commutativity of field multiplication: $ab = ba$
* Identity of field multiplication: There exists an element $1$ of $F$ such that $a1=a$
* Invertibility of field multiplication: For every $a$ in $F$, there exists an element $a^{-1}$ of $F$ such that $a(a^{-1})=1$
* Distributivity of field multiplication over field addition: $a(b+c)=ab+ac$
* Inequality of the field multiplication unit and the field addition unit: $0\neq1$

Examples of fields include the field of real numbers $\mathbb{R}$, and the field of complex of numbers $\mathbb{C}$. The rational numbers, algebraic numbers, and more exotic objects also form fields, but we'll mostly be focusing on $\mathbb{R}$ and sometimes $\mathbb{C}$.

Now we'll finally define $V$. A vector space is equipped with two additional operations $+$ (**vector addition**) and $\cdot$ (**scaling**) (we can omit the $\cdot$) which satisfies the following properties:
* Associativity of vector addition: $(\mathbf{u}+\mathbf{v})+\mathbf{w}=\mathbf{u}+(\mathbf{v}+\mathbf{w})$
* Commutativity of vector addition: $\mathbf{u}+\mathbf{v}=\mathbf{v}+\mathbf{u}$
* Identity of vector addition: There exists an element $\mathbf{0}$ of $V$ such that $\mathbf{v}+\mathbf{0}=\mathbf{v}$
* Inverses of vector addition: For every $\mathbf{v}$ in $V$, there exists an element $-\mathbf{v}$ such that $\mathbf{v}+(-\mathbf{v})=\mathbf{0}$
* Compatibility of field multiplication over scaling: $(ab)\mathbf{v}=a (b\mathbf{v})$
* Distributivity of scaling over vector addition: $a(\mathbf{u}+\mathbf{v})=a\mathbf{u}+a\mathbf{v}$
* Distributivity of scaling over field addition: $(a+b)\mathbf{v}=a\mathbf{v}+b\mathbf{v}$
* Identity of scaling: $1\mathbf{v}=\mathbf{v}$

Since vector addition operates on two vectors, and scaling operates on a scalar and a vector, this won't conflict with the notations for field addition and field multiplication.

Elements of $F$ are called **scalars** and are notated by lowercase italic letters like $a$ while elements of $V$ are called **vectors** and are notated by lowercase bold letters like $\mathbf{v}$.

#linear_algebra