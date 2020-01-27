# Eigenvectors and Eigenvalues

## What is an Eigenvector?

An **eigenvector** is a vector of a transformation that does not get 'knocked off' its original span after a linear transformation, aka they represent the basis vectors after a transformation. 

## What is an Eigenvalue?

An **eigenvalue** is the factor of how much the **eigenvectors** were squished or expanded, and this number is a scalar.

## Why are Eigenvectors useful?

They are useful because for example, if you have a 3D rotation, finding an eigenvector means you found the axis of rotation. *It is a great way to simplify a linear transformation.* Instead of saying, "here's a 3x3 matrix to describe this transformation!", you can get a 1x3 matrix describing the position of the eigenvector and how much it is rotating. Also, in this scenario the eigenvalue would be 1 since a simple rotation does not squish or stretch the vector itself.

## How to represent Eigenvectors and Eigenvalues
(because latex isn't working right now)

**A(v) = λ(v)**, where A is equal to the transformation matrix and v is equal to the eigenvector. λ is equal to the eigenvalue.

*You will want to find λ and v such that the statement is true.* This is usually awkward because you have to do two types of multiplication. (matrix vector and scalar multiplication).

Scalar multiplication with λ is basically having a 3x3 matrix with [λ 0 0] as the top, [0 λ 0], as the middle, and [0 0 λ] as the bottom. You can replace λ in all of these cases and call the matrix I (but you multiply this entire matrix by λ).

## How is this related to the determinant?

Simplified, you get this set-up:
**det(A - λI) = 0**

So that **(A - λI)(v) = 0**, where v is a non-zero vector.

What does this mean? It means that the eigenvalue will squish the vector into a simpler dimension, since the determinant must be 0.

## Finding the Eigenvalue

Simply take the matrix (in this example 2x2) of the eigenvector and subtract λ from the top left column and the bottom right. Then take the determinant of the matrix and see if it equals 0.

From there, you get a list of eigenvalues. But you have to plug them back into the matrix to see if the linear transformation will make the vector turn to [0 0]. 