# ADDITION OF ANGULAR MOMENTUM 

B. Zwiebach

December 12, 2013

## 1. Contents

1. Adding apples to oranges? 1

2. Adding two spin one-half angular momenta 3

3. Feynman-Hellman lemma $\quad 7$

4. Hyperfine splitting $\quad 9$

5. Spin-Orbit coupling $\quad 9$

![](https://cdn.mathpix.com/cropped/2023_10_06_07b1d7e63925c7ffce62g-01.jpg?height=52&width=1626&top_left_y=1069&top_left_x=263)

![](https://cdn.mathpix.com/cropped/2023_10_06_07b1d7e63925c7ffce62g-01.jpg?height=48&width=1629&top_left_y=1128&top_left_x=259)

5.3 Level splitting . . . . . . . . . . . . . . . . . . . . . . . 9

![](https://cdn.mathpix.com/cropped/2023_10_06_07b1d7e63925c7ffce62g-01.jpg?height=57&width=1626&top_left_y=1240&top_left_x=260)

6 General aspects of addition of angular momentum $\quad 9$

7 Hydrogen atom and hidden symmetry $\quad 9$

## 2. Adding apples to oranges?

We are going to be adding angular momenta in a variety of ways. We may add the spin angular momentum $\mathbf{S}$ of a particle to its orbital angular momentum $\mathbf{L}$. Or we may want to add the spin angular momentum $\mathbf{S}^{(1)}$ of a particle to the spin angular momentum $\mathbf{S}^{(2)}$ of another particle. At first sight we may feel like we are trying to add apples to oranges! For a given particle its spin angular momentum has nothing to do with spatial wavefunctions, while its orbital angular momentum does. How could we ever add such things? Adding the spins of two different particles also seems unusual if, for example, the particles are far-away from each other. Vectors that live at different places are seldom added: you don't typically add the electric field at one point to the electric field at another point: the sum has no obvious interpretation. This is even more severe in general relativity: you cannot add vectors that 'live' at different points of space-time. To add them you need a procedure to first bring them to a common point. Once they both live at that common point you can add them.

I want to make clear, however, that at a basic algebraic level all angular momenta are apples (granny smith, red-delicious, macintosh, fuji, etc.) and therefore they can be added and it is natural to add them. We are not adding apples to oranges; we are adding apples to apples! The physics requires it: we will see that energy eigenstates will also be eigenstates of operators in the sum of angular momenta. The mathematics allows it: the sum of angular momenta is an angular momentum acting in the appropriate tensor product. As we will see below, each angular momentum lives on a different vector space, but the sum finds a home in the tensor product of the vector spaces.

What is an angular momentum? It is a triplet $\hat{J}_{i}$ of Hermitian linear operators on some complex vector space $V$ satisfying the commutation relations

$$
\left[\hat{J}_{i}, \hat{J}_{j}\right]=i \hbar \epsilon_{i j k} \hat{J}_{k}
$$

As we have learned, this is a very powerful statement. When coupled with the requirement that no negative norm-squared states exist, it implies that $V$ can be decomposed into sums of representations of angular momentum, all of which are finite dimensional.

Let us now assume we have two angular momenta:

$$
\begin{aligned}
& \text { Hermitian operators } J_{i}^{(1)} \text { acting on } V_{1} \text { and satisfying }\left[\hat{J}_{i}^{(1)}, \hat{J}_{j}^{(1)}\right]=i \hbar \epsilon_{i j k} \hat{J}_{k}^{(1)} \\
& \text { Hermitian operators } J_{i}^{(2)} \text { acting on } V_{2} \text { and satisfying }\left[\hat{J}_{i}^{(2)}, \hat{J}_{j}^{(2)}\right]=i \hbar \epsilon_{i j k} \hat{J}_{k}^{(2)}
\end{aligned}
$$

Our claim is that the 'sum' of angular momenta is an angular momentum in the tensor product:

$$
\hat{J}_{i} \equiv \hat{J}_{i}^{(1)} \otimes \mathbf{1}+\mathbf{1} \otimes \hat{J}_{i}^{(2)} \text { satisfies }\left[\hat{J}_{i}, \hat{J}_{j}\right]=i \hbar \epsilon_{i j k} \hat{J}_{k} \text { acting on } V_{1} \otimes V_{2} \cdot
$$

Certainly the sum operator, as defined above, is an operator on $V_{1} \otimes V_{2}$. It is in fact a Hermitian operator on $V_{1} \otimes V_{2}$. We just need to check that the commutator holds

$$
\begin{aligned}
{\left[\hat{J}_{i}, \hat{J}_{j}\right] } & =\left[\hat{J}_{i}^{(1)} \otimes \mathbf{1}+\mathbf{1} \otimes \hat{J}_{i}^{(2)}, \hat{J}_{j}^{(1)} \otimes \mathbf{1}+\mathbf{1} \otimes \hat{J}_{j}^{(2)}\right] \\
& =\left[\hat{J}_{i}^{(1)} \otimes \mathbf{1}, \hat{J}_{j}^{(1)} \otimes \mathbf{1}\right]+\left[\mathbf{1} \otimes \hat{J}_{i}^{(2)}, \mathbf{1} \otimes \hat{J}_{j}^{(2)}\right],
\end{aligned}
$$

since the mixed terms, which represent commutators of the operators in the different spaces vanish:

$$
\left[\hat{J}_{i}^{(1)} \otimes \mathbf{1}, \mathbf{1} \otimes \hat{J}_{j}^{(2)}\right]=0, \quad\left[\mathbf{1} \otimes \hat{J}_{i}^{(2)}, \hat{J}_{j}^{(1)} \otimes \mathbf{1}\right]=0 .
$$

(If this is not 'obvious', think about it and do the one-line computation that will make it obvious!). Writing out the commutators we see that (1.4) becomes

$$
\left[\hat{J}_{i}, \hat{J}_{j}\right]=\left[\hat{J}_{i}^{(1)}, \hat{J}_{j}^{(1)}\right] \otimes \mathbf{1}+\mathbf{1} \otimes\left[\hat{J}_{i}^{(2)}, \hat{J}_{j}^{(2)}\right]
$$

We can now use the independent algebras of angular momentum to find

$$
\begin{aligned}
{\left[\hat{J}_{i}, \hat{J}_{j}\right] } & =i \hbar \epsilon_{i j k} \hat{J}_{k}^{(1)} \otimes \mathbf{1}+i \hbar \epsilon_{i j k} \mathbf{1} \otimes \hat{J}_{k}^{(2)} \\
& =i \hbar \epsilon_{i j k}\left(\hat{J}_{k}^{(1)} \otimes \mathbf{1}+\mathbf{1} \otimes \hat{J}_{k}^{(2)}\right) \\
& =i \hbar \epsilon_{i j k} \hat{J}_{k}
\end{aligned}
$$

which is what we set out to prove. It is important to note that had we added the two angular momenta with some arbitrary coefficients we would not have got an angular momentum. Indeed, suppose we use two non-zero complex constants $\alpha$ and $\beta$ and write

$$
\tilde{J}_{i} \equiv \alpha \hat{J}_{j}^{(1)} \otimes \mathbf{1}+\beta \mathbf{1} \otimes \hat{J}_{j}^{(2)} .
$$

If either constant is zero we are not really summing. The commutator calculation above this time yields

$$
\left[\tilde{J}_{i}, \tilde{J}_{j}\right]=i \hbar \epsilon_{i j k}\left(\alpha^{2} \hat{J}_{k}^{(1)} \otimes \mathbf{1}+\beta^{2} \mathbf{1} \otimes \hat{J}_{k}^{(2)}\right) .
$$

We have an algebra of angular momentum if the operator in parenthesis is $\tilde{J}_{k}$. This requires $\alpha^{2}=\alpha$ and $\beta^{2}=\beta$. Since neither $\alpha$ nor $\beta$ is zero, the only solution is $\alpha=\beta=1$. This confirms that we are using in (1.3) the unique way to add two angular momenta to form a new angular momentum.

By the same arguments that hold for any angular momentum on a vector space, the space $V_{1} \otimes V_{2}$ can be decomposed into sums of representations of the algebra of total angular momentum. This property gives us a powerful tool to understand the spectrum of the Hamiltonian in the physical state space $V_{1} \otimes V_{2}$.

## 3. Adding two spin one-half angular momenta

To set up the notation recall that for a spin one-half particle and spin operators $\mathbf{S}$ we write

$$
\mathbf{S}^{2}|s, m\rangle=\hbar^{2} s(s+1)|s, m\rangle, \quad \hat{S}_{z}|s, m\rangle=\hbar m|s, m\rangle, \quad \text { with } s=\frac{1}{2} \text {, and } m= \pm \frac{1}{2} \text {. }
$$

The states that span the vector space are thus

$$
\left|\frac{1}{2}, \frac{1}{2}\right\rangle, \quad\left|\frac{1}{2},-\frac{1}{2}\right\rangle,
$$

states that we used to label as $|+\rangle$ and $|-\rangle$, respectively. The action of $\mathbf{S}^{2}$ on any of these states gives $\frac{3}{4} \hbar^{2}$ and the action of $\hat{S}_{z} / \hbar$ gives $\frac{1}{2}$ on the first and $-\frac{1}{2}$ on the second.

We now consider the case in which our system features two spin one-half particles. For the first particle we have the triplet of spin operators $\mathbf{S}^{(1)}$ acting on the vector space $V_{1}$ spanned by

$$
\left|\frac{1}{2}, \frac{1}{2}\right\rangle_{1}, \quad\left|\frac{1}{2},-\frac{1}{2}\right\rangle_{1},
$$

For the second particle we have the triplet spin operators $\mathbf{S}^{(2)}$ acting on the vector space $V_{2}$ spanned by

$$
\left|\frac{1}{2}, \frac{1}{2}\right\rangle_{2}, \quad\left|\frac{1}{2},-\frac{1}{2}\right\rangle_{2} .
$$

We now form the total spin

$$
\hat{S}_{i} \equiv \hat{S}_{i}^{(1)} \otimes \mathbf{1}+\mathbf{1} \otimes \hat{S}_{i}^{(2)}
$$

which we write, for brevity as

$$
\hat{S}_{i}=\hat{S}_{i}^{(1)}+\hat{S}_{i}^{(2)}, \text { for example, } \hat{S}_{z}=\hat{S}_{z}^{(1)}+\hat{S}_{z}^{(2)},
$$

with the understanding that each operator on the right-hand sides acts on the appropriate factor in the tensor product. The state space for the dynamics of the two particles must contain the tensor product $V_{1} \otimes V_{2}$ (more spaces might be needed if the particles have orbital angular momentum or they are moving). As we learned before, $V_{1} \otimes V_{2}$ is a four-dimensional complex vector space spanned by the products of states in (2.3) and (2.4):

$$
\left|\frac{1}{2}, \frac{1}{2}\right\rangle_{1} \otimes\left|\frac{1}{2}, \frac{1}{2}\right\rangle_{2}, \quad\left|\frac{1}{2}, \frac{1}{2}\right\rangle_{1} \otimes\left|\frac{1}{2},-\frac{1}{2}\right\rangle_{2}, \quad\left|\frac{1}{2},-\frac{1}{2}\right\rangle_{1} \otimes\left|\frac{1}{2}, \frac{1}{2}\right\rangle_{2}, \quad\left|\frac{1}{2},-\frac{1}{2}\right\rangle_{1} \otimes\left|\frac{1}{2},-\frac{1}{2}\right\rangle_{2} .
$$

It must be possible to organize these states into finite-dimensional representations of the total spin angular momentum, which is well-defined acting on these states. We have four basis states so the possibilities for multiplets of total spin $s$ are

1. Four singlets $(s=0)$.
2. Two doublets $\left(s=\frac{1}{2}\right)$.
3. One doublet $\left(s=\frac{1}{2}\right)$ and two singlets $(s=0)$.
4. One triplet $(s=1)$ and one singlet $(s=0)$.
5. One $s=\frac{3}{2}$ multiplet.

It may be instructive at this point if you pause to make sure no other option exists and then to consider which option is the only likely to be true! Guess it!

The main clue is that the states in the tensor product are eigenstates of $\hat{S}_{z}$, the total $z$-component of angular momentum. We see by inspection of (2.7) that the possible values of $\hat{S}_{z} / \hbar$ and $+1,0$, and -1 . Since we have a state with $m=+1$ and no state with higher $m$ we must have a triplet $s=1$. Thus the only option is the fourth one listed above: a triplet and a singlet. This is written as

$$
\left(s=\frac{1}{2}\right) \otimes\left(s=\frac{1}{2}\right)=(s=1) \oplus(s=0)
$$

Note that in the left-hand side we have the tensor product of the two state spaces, but in the right-hand side the direct sum of the representations of total spin angular momentum. This is a fundamental result and is written more briefly as

$$
\frac{1}{2} \otimes \frac{1}{2}=1 \oplus 0
$$

Let us understand this very explicitly by organizing the basis states according to the eigenvalue $m$ of $\hat{S}_{z} / \hbar$. We readily observe that

$$
\begin{array}{ll}
m=1: & \left|\frac{1}{2}, \frac{1}{2}\right\rangle_{1} \otimes\left|\frac{1}{2}, \frac{1}{2}\right\rangle_{2}, \\
m=0: & \left|\frac{1}{2}, \frac{1}{2}\right\rangle_{1} \otimes\left|\frac{1}{2},-\frac{1}{2}\right\rangle_{2}, \quad\left|\frac{1}{2},-\frac{1}{2}\right\rangle_{1} \otimes\left|\frac{1}{2}, \frac{1}{2}\right\rangle_{2}, \\
m=-1: & \left|\frac{1}{2},-\frac{1}{2}\right\rangle_{1} \otimes\left|\frac{1}{2},-\frac{1}{2}\right\rangle_{2} .
\end{array}
$$

