Dependencies | Dependents
------------ | ------------
N/A | [[Abstract vectors]]

Linear algebra is fundamentally about things which can be added and scaled, and functions which preserve addition and scaling, so we will briefly define linearity.

A function $f$ is **linear** if and only if it satisfies the following properties:
* $f(x+y)=f(x)+f(y)$
* $f(ax)=af(x)$

I'm intentionally being vague about what $f$, $x$, $y$, $a$, and addition and multiplication mean here. Really, all you need to know is that $a$ is some factor by which you can scale $x$ or $y$, which is just multiplication.

We can also define an analogous property for functions of arbitrary numbers of variables. 

A function is called **multilinear** if and only if when you fix all inputs except one, the result is a linear function. In the case where it takes only two variables, it is also called **bilinear**.

#linear_algebra 