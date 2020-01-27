# Linear Transformations in 2D

## Linear Transformations

A transformation is a function. You take some vector and then spit out another vector. Input: vector, output: vector.

A transformation is linear if:
* All lines remain lines.
* The origin remains in place.

In other words, ***gridlines remain parallel and equally spaced***. 

For example, linear transformations can be:
* Rotation around the origin
* Multiplying all vectors by a scalar

## Recording Transformations in 2D
  
To find the changes in vectors after transformations, you only need to record changes in the basis vectors, which will be a 2x2 Matrix. These are the coordinates where both these unit vectors land. This is because all vectors can be described as those vectors multiplied by certain scalars. The transformed coordinates of ihat and jhat are on the left and right columns of the matrix respectively.

$$ \text{Transformed } \hat{i}, \hat{j} =
\begin{bmatrix}
3 & 2 \\
-2 & 1
\end{bmatrix} $$

Given the coordinates of the vector you're transforming (for example x, y = [1, 2]), the transformed vector is equal to:

$$ \text{Transformed }\vec{v}=(1)(\text{Transformed }\hat{i})+(2)(\text{Transformed }\hat{j}) $$

***All you need are the transformed unit vector values.*** Since gridlines will remain parallel and equally spaced, you can deduce where the vector must go given the *transformed unit vectors* for the coordinate system. Then, you can plug in the transformed unit vector values into the transformed vector.

$$ \text{Transformed }\vec{v}=(1)(3)\vec{i}+(2)(2)\vec{j}, (1)(-2)\vec{i} + (2)(1)\vec{j} $$

If you are given any vector, you can calculate where it lands using the formula above!

### Example: 90 degree rotation clockwise.

Our transformed matrix equals:
$$ \text{Transformed } \hat{i}, \hat{j} =
\begin{bmatrix}
0 & 1 \\
-1 & 0
\end{bmatrix} $$

