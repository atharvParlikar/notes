Karnaugh map is a method of simplifying boolean algebra expressions.
kmap reduces the need for extensive calculations by using the pattern recognition abilities of humans.

### Example

![[Pasted image 20230123151405.png]]
This table and following function are notations describing the same function in unsimplified Boolean algebra, using boolean variables A,B,C,D

$f(A,B,C,D) = \Sigma m_{i}, i \in \{6,8,9,10,11,12,13,14\}$ 

#### Construction
In the example above, the 4 input variables can be combined in 16 different ways, so the truth table has 16 rows, and the kmap has 16 positions.
The kmap grid is therefore arranged in 4x4 grid.
Note: The row and column indices are orderd in [[gray code]]

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/1a/K-map_minterms_A.svg/220px-K-map_minterms_A.svg.png" style="background-color: white; height: 200px">

This is basically kmap representation of above function,
to minimize it you might need to look at [[Minimization of combinational circuites using k-maps]]
