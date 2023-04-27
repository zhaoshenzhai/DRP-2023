1. Title page
    - Hi everyone, so my project is on the interface between topological manifolds and complex manifolds.
    - Specifically, we worked with surfaces, so $2$-dimensional topological manifolds, and we asked in how many ways can we turn a surface into a complex manifold.
    - In other words, given a surface, how many different choices of complex coordinates are there for the surface?
    - To illustrate, let's look at a simple example, which is the plane $\R^2$.
2. $\l(x,y\r)\mapsto x+iy$
    - One way to give $\R^2$ complex coordinates is the obvious one by assigning a pair $\tpl{x,y}$ the complex number $x+iy$.
    - However, we can assign coordinates in any reasonable way we want, so why not something like this?
3. $\l(x,y\r)\mapsto x-iy$
    - Here, we basically reflected $\R^2$ about the $x$-axis, which gives us different complex coordinates on $\R^2$.
4. Biholomorphisms
    - However, this is not really intersecting, and the difference between those two complex coordinates is basically convention.
    - In fact, we can make this precise by saying that there is an isomorphism that preserve the complex structure, which we call a biholomorphism.
    - We say that $\R^2$, equipped with the top complex structure, is biholomorphic to $\R^2$ but equipped with the bottom one.
    - So those two are actually the same.
6. Refined question
    - So instead of asking about literally how many complex coordinates there are, we only ask up to biholomorphism.
    - It turns out that there are two complex structures on $\R^2$ up to biholomorphism, and they are...
8. Two complex structures on $\R^2$
    - The one that we saw, which is the usual one, and the upper-half plane.
    - Those two are fundamentally different complex coordinates on $\R^2$, as there are no biholomorphisms between the two.
    - In fact those are the only two complex coordinates on $\R^2$.
10. Riemann surfaces
    - Now lets do the same for surfaces in general.
    - From Haoyang's talk, we saw that surfaces basically look like this and can be described mathematically as topological manifolds.
    - A Riemann surface is basically a surface after we've assigned complex coordinates to it.
    - So another way to ask our question is in how many ways can be make a surface into a Riemann surface?
    - We'll only be looking at compact surfaces, which are basically surfaces that are closed and bounded (so everything there except for $\R^2$.)
12. Classification of surfaces
    - There's a theorem from topology that says that the only difference between two compact surfaces is the number of holes that it has.
    - The number of holes is called the genus of the surface.
    - For example, the sphere with one handle is homeomorphic to the torus, since they both have one hole.
14. Topological torus
    - Let's now answer the question for the torus.
    - From Haoyang's talk, we saw that a torus is obtained by quotienting the plane by a lattice.
    - A lattice partitions the plane into parallelograms, and the torus is obtained by glueing the sides.
    - Using different lattices will change the two radii of the torus, but, topologically, they are all the same.
    - However, it turns out that we can give the torus different complex coordinates, and the choices of complex coordinates are determined by the lattices.
    - So we need to determine how do different lattices give rise to different complex coordinates.
16. Scaling/rotating doesn't matter
    - There's a theorem from complex analysis that holomorphic maps preserve angles.
    - So, intuitively, if we do anything to the plane that preserve angles, like scaling and rotating, the resulting tori should be biholomorphic.
    - Essentially, if the lattice is spanned by $\omega_1$ and $\omega_2$, only their ratio matters.
    - Thus every complex tori can be written as $\C$ quotient by a lattice of that form, which only depends on $\tau$.
    - This $\tau$, which lies in the upper-half plane of $\C$, is the ratio of the $\omega$'s, and we call the resulting torus $X_\tau$.
18. Fundamental domain and the moduli space
    - However, it turns out that different $\tau$'s can actually give the same torus, which is quite surprising.
    - Pictorially, consider the upper-half plane and fix a $\tau$ in the shaded region.
    - If we shift this $\tau$ one unit to the right, the resulting tori $X_\tau$ and $X_{\tau'}$ are actually biholomorphic.
    - It turns out that if we map $\tau$ to any of those red points, the resulting tori are all biholomorphic.
    - Within any one of the triangular regions, like the shaded region, varying $\tau$ will give different complex tori, which you can think of making the torus skinnier or fatter. This region, which is called the fundamental domain, parametrizes the different complex coordinates on the torus.
    - Since we only want to look at one of those regions (the others are in some sense duplicates), we take the quotient under the group action that sends $\tau$ to the other red points. This quotient, which uniquely parametrizes the complex coordinates of the torus, is called the moduli space of the torus.
21. $\H/\PSL\l(2,\Z\r)$
    - Explicitly, the group of such functions, labelled $\gamma$ here, is called the modular group.
    - We've basically proved that two tori $X_\tau$ and $X_{\tau'}$ are biholomorphic iff $\tau$ and $\tau'$ are related by an element of the modular group, so the moduli space of the torus is $\H/\PSL\l(2,\Z\r)$.
    - This answers the question for the torus, but to reiterate:
    - The $\H$ comes from the fact that every lattice is determined by some $\tau$ in the upper-half plane, which is the ratio of the $\omega$'s.
    - And the modular group removes redundant $\tau$'s that generate the same torus.
24. Riemann sphere
    - Let's also quickly talk about the sphere, which turns out to admit a unique complex coordinate.
    - What this means is that every sphere is biholomorphic to each other, which is pretty surprising.
    - The proof for this is hard, but it essentially goes like this. Let's fix a particular complex coordinate and call the resulting sphere the Riemann sphere $\RS$.
    - Our task is to show that every other sphere $X$ is biholomorphic to the Riemann sphere.
    - The first thing we proved is that if we can find a meromorphic function with a single simple pole on $X$, then $X$ is biholomorphic to the Riemann sphere.
    - To find such a function, we first tried to define it locally as $1/z$ and then analytically continue it to the rest of $X$, but this didn't work out.
    - Instead, what we needed was tools from cohomology, which give us sufficient conditions to patch up local functions into global ones.
    - This worked, which proves the theorem.
    - This is a significant result in the theory of Riemann surfaces and is part of the so-called Uniformization Theorem.

This gives us one way of viewing $\R^2$ as $\C$. Any such way of viewing $\R^2$ as $\C$ is called a choice of complex coordinates or complex structures on $\R^2$.
