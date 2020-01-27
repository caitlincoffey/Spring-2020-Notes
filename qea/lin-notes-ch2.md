# Linear Combination, Span, and the Basis of a Vector Space

### Unit Vectors and Basis Vectors
Each number in the matrix is a scalar mutiplied by a unit vector. Therefore vectors can be displayed in this format because unit vectors have a magnitude of 1 along each specific axis. 

$$ \vec{A}=(A_x)\hat{i} + (A_y)\hat{j}+(A_z)\hat{k} $$

Unit vectors are also called the **basis vectors** because they are essential to the coordinate system. The matrix provided simply scales those vectors.

### Linear Combination

When you add two vectors and multiply each vector by its own scalar, that is called **Linear Combination.**

$$ a\vec{v} + b\vec{w} $$ 

### Span

If you fix one vector (ie: scalar remains constant), you will create a line with all the possibilities of what the scalar could be with the other vector. If you do not fix either, you can theoretically reach any point on the plane. This is called the **span**. 

The span is the set of all possible **Linear Combinations**. It is represented as a space on a coordinate system, which could take shape as a line or a plane or even all the space on the coordinate system.

### Viewing Vectors as Points

You can view vectors as a point in space. Assuming their tail is at the origin, you can view the head as the 'point' in space. 

If you have a single vector, it's convenient to think of it as an arrow. 

If you have a point, think of them as points. This is because some of their spans could be lines (for example, if lines have same direction).

### Vectors in 3D

If you have two 3D vectors, what is their span? If you scale the two vectors in some way, you get a 2D plane. Consider it like turning a knob.

A linear combination of three 3D vectors usually 'unlocks' access to all 3D vectors. It moves the 2D plane so that it can access the full 3D dimensions of the space.

### Linearly Dependent and Independent
**Linearly dependent** means that one vector can be described as a combination of two vectors. It does not add another dimension to the span.

**Linearly independent** means that the addition of one vector adds dimension to the span.

### Basis of a Vector Space

The **basis** of any vector space (space on a plane) is a set of linearly independent vectors that span the full space. 
*For example, a 2D plane is a set of two 3D vectors.


