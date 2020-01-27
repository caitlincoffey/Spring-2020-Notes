# Linear Algebra, Vectors, and Matrices

## Rows and Columns

What does it mean when a matrix is 2 x 1? Or 1 x 2? *The **first number** refers to the number of **rows** in the matrix, while the **second** refers to the number of **columns***. Think of it as ***FR, SC***. France, South Carolina?

$$ \text{2 x 1 matrix} = \begin{bmatrix}
1 \\
-2
\end{bmatrix} $$

$$ \text{1 x 2 matrix} = \begin{bmatrix} 1 & -2 \end{bmatrix}$$

## The Transpose of a Vector

Converting a column vector to a row vector is called taking the **transpose** of the vector. You can denote this with a superscript T on the top-right corner of your vector. For example:

$$ \text{u}^{T} =
\begin{bmatrix}
3 \\
-2
\end{bmatrix} = [3 -2] $$

**Refer to this formula when transposing matrices**. Since the shape of the matrix changes when you transpose it, this is super important to remember!

$$ (Av)^{T} = v^{T}A^{T} $$



## Taking the Product of a Column Vector and Row Vector

Use the follow formula to take the product of a column vector with a row vector.

$$ \text{uv} = [p q r]
\begin{bmatrix}
x \\
y \\
z 
\end{bmatrix} =px+qy+zr $$

Also, if you take the dot product of a vector with a transposed vector, the results remain the same. So don't worry about transposing vectors and then taking the dot product and fearing the results will be different than just not transposing!

## Finding the Dot Product of Two (Column or Row) Vectors

Remember that the dot product tells us how 'aligned' two vectors are to each other. If the vectors are perpendicular, then the dot product is equal to 0. If the dot product is 1, the vector is parallel. Essentially you are being given a scalar value as a product. This is because of the following equation:

$$ \vec{u}\cdot\vec{v} = |\vec{u}||\vec{v}|\cos(\theta) $$
$$ \cos(90{\degree}) = 0, \text{ so yeah}$$

But there is also this equation which is equally important:

$$ v·w= v_1w_1+v_2w_2+· · ·+v_nw_n $$

## What is the difference between a Vector and Matrix?

Vectors and matrices are basically lists of numbers. Matrices can have any number of columns (m) or rows (n). ***Vectors are specific examples of matrices in that they either have a single row (1 x n, row vectors) or a single column (m x 1, column vectors).***

## How Do You Represent Matrices and Vectors?

You represent a matrix with an *uppercase letter*, such as A or G. You represent a vector with a *lowercase letter* (no, you do not necessarily need the vector notation as we are using them as lists).

## Matrix and Vector Multiplication

There are two ways at looking at multiplying vectors with matrices. *Since you are using the dot product, you can use transverse vectors to your own liking*. This particularly comes in handy when a column of a matrix matches up with the row of a vector. You can simply view the output vector as a linear combination of the columns of the matrix with the rows of the vector. The other option is to view each row of the matrix as its seperate entity and use the dot product for each row.

## Rotation Matrix (Linear Transformation)

The following matrix rotates any given vector counter-clockwise (or clockwise, if given theta is negative/angle value is negative):

$$ \text{R} = 
\begin{bmatrix}
\cos(\theta) & -sin(\theta)\\
\sin(\theta) & cos(\theta) \\
\end{bmatrix} $$

## Writing Matrices in Matlab

It's very easy to create and use matrices/vectors in Matlab. To create a matrix with two rows and columns, simply use this syntax:

`A = [a c; b d]`

***Semicolons seperate rows.*** To create a *row vector* that's 1 x 4, simply type a command like this one:

`v = [a; b; c; d]`

A *column vector* would look like this.

`w = [a b c d]`

## Plotting Matrices in Matlab

Use the `plot` function to plot a scatter plot. You can plot two matrices (given the same dimensions) with this function.

The `help` function is also super nice. *Type `help plot` to get information about the plot function!*

## For loops and function of them

Matlab's `for` loops are good for repeating a set of commands multiple times. For example, the code below will take a list of integers (1 to 3), square them, and store them in vector `v`.

    for n=1:3
        v(n) = n^2;
    end

If you wanted to print out the value of `v`, you could simply type `v` below the loop without a semicolon to suppress the output. If you wanted to graph `v`, simply use the command `plot(v)`.

To make a 2x4 matrix (two columns, 4 rows), with a function determining the 2nd column, you can use the `for` loop to make the matrix:

    for n=1:4
        M_squares(n,1) = n
        M_squares(n,2) = n^2
    end

## Multiplying Two Matrices

In general, given two matrices (A, B), with A having *m x n* columns and B having *p x q* columns, you need **n = p (columns for A equal to rows for B)** for **C = AB to be defined**. 

**C = AB is equal to m x q**. *For the q columns of matrix C, those are the q vectors that come from **multiplying matrix A with the vectors for each column of B.*** For example:

$$ A = \begin{bmatrix}
2 & 1 \\
3 & -1
\end{bmatrix} B = \begin{bmatrix} 1 & 5 \\ -2 & 3 \end{bmatrix} $$

For these given matrices, **C** is equal to the following:

$$ C = \begin{bmatrix} (2)(1) + (1)(-2) & (2)(5) + (1)(3) \\ (3)(1) + (-1)(-2) & (3)(5) + (-1)(3) \end{bmatrix} = \begin{bmatrix} 0 & 13 \\ 5 & 12 \end{bmatrix} $$

## Types of Matrices
Look at notebook for a better explanation of this topic. 

*There are: **Square Matrices, Rectangular Matrices, Diagonal Matrices, Identity Matrices,*** and ***Symmetric Matrices.***
