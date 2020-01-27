# Composition Matrices

### What is a Linear Transformation?

Linear Transformations are matricies that can effectively be described as transformations of vectors. When you apply one to a vector you are transforming it. Here are some examples of transformations you can apply:

**90 degree rotation clockwise.**
$$ \text{Rotation 90°} \hat{i}, \hat{j} =
\begin{bmatrix}
0 & 1 \\
-1 & 0
\end{bmatrix} $$

**Shear transformation**
$$ \text{Shear } \hat{i}, \hat{j} = 
\begin{bmatrix}
1 & 2 \\
0 & 1
\end{bmatrix} $$

## Composition Matrices

Composition matrices are the product of two or more matrices (aka transformations). This is useful if you are applying more than 1 transformation to a vector. 

Instead of applying the transformations separately, you can find the composition matrix by finding