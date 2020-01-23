# Daily Notes

## 01/17/20
R<sup>*</sup> = [r<sup>*</sup>]<sub>nq</sub> = BC

S<sup>*</sup> = [s<sup>*</sup>]<sub>mq</sub> = A(BC)

S<sub>ij</sub><sup>*</sup> = [s<sup>*</sup>]<sub>mq</sub> = A(BC)


3)A(B + C) = AB + AC

4)(B + C)A = BA + CA

5)AB = 0 => A=0 or B=0

    Ex: let A =|4 2| , B = |3 -4|
               |2 1|,      |-6 8|

        AB = |0 0|
             |0 0|<sub>2x2</sub>

### Transpose:
Definition: if A = [a<sub>ij</sub>]<sup>i=1...n</sup><sub>j=1...p</sub> is a nxp matrix then the transpose of A denoted by A<sup>T</sup>= [a<sub>ji</sub>] is an pxn matrix.

    Ex: A = |1 2 3|,    A<sup>T</sup>|1 4|
            |4 5 6|                  |2 5|
                                     |3 6|

### Transpose properties
1) (A<sup>T</sup>)<sup>T</sup> = A

2) 	(lambda(A))<sup>T</sup> = lambda(A)<sup>T</sup>

3) (A + B) <sup>T</sup> = A<sup>T</sup> + B<sup>T</sup>

4) (AB)<sup>T</sup> = B<sup>T</sup>A<sup>T</sup>

5) (ABC)<sup>T</sup> = [(AB)C]<sup>T</sup> = C<sup>T</sup>(AB)<sup>T</sup> = C<sup>T</sup>A<sup>T</sup>B<sup>T</sup>

### Special matrix


### Diagonal matrix
Is a square matrix with all elements except those on the main diagonal equal to zero.

![](./../photos/diagonal.png)

### Identity matrix
Diagonal matrix with all diagonal element equal to 1.

![](./../photos/identitymatrix.png)

A * I = A, I * A = A

### Symmetric Matrices
Definition:

- 1) symmetric Matrix A = A<sup>T</sup>
- 2) skew-symmetric matrix A = -A<sup>T</sup>

![](./../photos/symmetricmatrix.jpg)

### Lower/Upper triangular matrices:

A matrix A = [a<sub><ij</sub>] is called
 - lower triangular if a<sub>ij</sub> = 0, for j>i
 - upper triangular if a<sub>ij</sub> = 0, for i>j

 ![](./../photos/triangularmatrix.png)

### Linear system of equations.

a<sub>11</sub>x<sub>1</sub> + a<sub>12</sub>x<sub>2</sub> + ... + a<sub>1n</sub>x<sub>n</sub> = b<sub>1</sub>

---

## 01/22/20 The system of equations can be written as augmented matrix:

A = [A;B]

For homogenous system there is at least one solution.
![](./../photos/homogenous-system.jpg)

### Gaussian Elimination
1. two rows (r<sub>i</sub><->r<sub>i</sub>)
2. a scalar times one row (r<sub>i</sub>=(scalar)r<sub>i</sub>)
3. Add one row by a scalar times another row (r<sub>i</sub>= r<sub>i</sub> + (scalar)r<sub>i</sub>)

x<sub>1</sub> + 3x<sub>2</sub> = 4 A = |1 3 |4| <br>
2x<sub>1</sub> - x<sub>2</sub> = 1 &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; |2 -1|1| <br>
3x<sub>1</sub> + 2x<sub>2</sub> = 5&nbsp; &nbsp; &nbsp;&nbsp;|3  2|5|<br>
5x<sub>1</sub> + 15x<sub>2</sub> = 20&nbsp;&nbsp;&nbsp;|

### Goal Gaussian Elimination

1. an upper triangular form.
2. main diagonal to be unity.

### Basic Principles

1. Completely reduce one column before considering another column.
2. work on column in order from left to right.

### Types of solutions:
1. no solutions
* No solutions when bottom row has all zeroes but right column is Non-zero
2. unique solutions
* if not a `no solution` and # of pivot == # of variables
3. infinite solutions
* if not a `no solution` and # of pivot < # of variables

### Row Echelon Form
![](./../photos/Row-Echelon-Form.png)

### pivot
Want to follow pivot when writing down answer<br>
x<sub>1</sub> = x<sub>2</sub> - 1<br>
x<sub>2</sub> = infinite solutions<br>
x<sub>3</sub> = 1

![](./../photos/pivot.jpg)


### left column is not Echelon Form right column is Echelon Form
