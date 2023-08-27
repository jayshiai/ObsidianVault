#2ndYear #Maths 
Example

$$
x-y+2z=3
$$
$$
x+2y+3z=5
$$
$$
3x-4y-5z = -13
$$
Lets create matrix in for
$$AX = B$$
We'll create Augmented matrix 
$$(A:B) = 
\begin{bmatrix}
1 & -1 & 2: & 3  \\
1 & 2 & 3: & 5 \\
3 & -4 & -5: & -13
\end{bmatrix}
$$

Through row transformation, we'll get matrix in  format :-

$$
(A:B) = 
\begin{bmatrix}
1 & -1 & 2: & 3  \\
0 & 3 & 1: & 2 \\
0 & 0 & -32: & -64
\end{bmatrix}
$$
i.e. zeros in lower triangle.

This yields following equations:
$$x-y+2z = 3$$
$$3y+z=2$$
$$-32z=-64$$
On solving we get :
$$x=-1$$
$$y=0$$
$$z=2$$
