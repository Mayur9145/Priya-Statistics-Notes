# Linear Algebra Notes

## 1. Linear Algebra
Linear algebra is the branch of mathematics concerning linear equations, linear functions, and their representations through matrices and vector spaces. It's fundamental for data science, machine learning, and optimization problems.

## 2. Scalars and Vectors

### Scalars
A scalar is a single number used to represent magnitude (or size). It has no direction. Examples include temperature, time, and distance.

### Vectors
A vector is a mathematical object that has both magnitude and direction. In physics and engineering, vectors represent quantities such as velocity and force.

**Example**:
A vector in 3D space:

v = [2, 4, 6]


This vector has three components in the x, y, and z directions.

## 3. Eigenvalues and Eigenvectors

### Eigenvalue
An eigenvalue is a scalar that indicates how much the corresponding eigenvector is stretched or shrunk during a linear transformation. If \( A \) is a square matrix, then for a given vector \( v \), the equation is:


A * v = λ * v


Where:
- \( A \) is a square matrix.
- \( v \) is the eigenvector.
- \( λ \) is the eigenvalue.

### Eigenvector
An eigenvector is a vector that does not change its direction during a linear transformation. It can be scaled by its associated eigenvalue.

**Example**:
For a 2x2 matrix \( A \):

A = [[4, 1], [2, 3]]


The eigenvalue \( λ = 5 \), and its corresponding eigenvector can be \( v = [1, 1] \).

## 4. Matrix Operations

### Matrix Addition
You can add matrices by adding their corresponding elements if they have the same dimensions.

**Example**:

A = [[1, 2], [3, 4]] B = [[5, 6], [7, 8]] A + B = [[6, 8], [10, 12]]



### Matrix Multiplication
Matrix multiplication is done by multiplying the rows of the first matrix by the columns of the second.

**Example**:

A = [[1, 2], [3, 4]] B = [[5, 6], [7, 8]] A * B = [[19, 22], [43, 50]]


### Transpose of a Matrix
The transpose of a matrix flips it over its diagonal, swapping rows with columns.

**Example**:
A = [[1, 2, 3], [4, 5, 6]] Transpose(A) = [[1, 4], [2, 5], [3, 6]]



## 5. Orthogonality
Two vectors are orthogonal if their dot product is zero, meaning they are at a 90-degree angle.

**Example**:
Let vectors \( u = [1, 0] \) and \( v = [0, 1] \). Their dot product:

u . v = 10 + 01 = 0


Since the dot product is zero, the vectors are orthogonal.

## 6. Projections
The projection of vector \( u \) onto vector \( v \) is given by:


Proj_v(u) = (u . v / v . v) * v


Where:
- \( u . v \) is the dot product.
- \( v . v \) is the magnitude squared of \( v \).

**Example**:
Let \( u = [3, 4] \) and \( v = [1, 2] \):


Proj_v(u) = [(31 + 42) / (11 + 22)] * [1, 2] = [11 / 5] * [1, 2] = [2.2, 4.4]



## 7. Norms and Vector Magnitude

### Norm of a Vector
The norm (or length) of a vector \( v \) is a measure of its magnitude. The most common norm is the Euclidean norm, given by:


||v|| = sqrt(v_1^2 + v_2^2 + ... + v_n^2)


**Example**:
For vector \( v = [3, 4] \):
||v|| = sqrt(3^2 + 4^2) = sqrt(9 + 16) = sqrt(25) = 5



### Vector Magnitude
The magnitude of a vector is the length or size of the vector. For a 3D vector \( v = [x, y, z] \):
|v| = sqrt(x^2 + y^2 + z^2)



**Example**:
For vector \( v = [2, 3, 6] \):

|v| = sqrt(2^2 + 3^2 + 6^2) = sqrt(4 + 9 + 36) = sqrt(49) = 7


## 8. Vector Dimensions
The dimension of a vector refers to the number of components in it. A 3-dimensional vector has three components (x, y, z).

**Example**:
A vector in 2D:
v = [5, 9]


A vector in 3D:
v = [1, 2, 3]


## 9. Rad (Radians)
Radian is a unit of angular measure. One radian is the angle subtended at the center of a circle by an arc whose length is equal to the circle's radius.

**Example**:
In a circle with radius \( r = 1 \), the angle subtended by an arc of length \( r \) is 1 radian.
Angle in radians = arc length / radius









