# Matrix-Math

## Synopsis
This bash script takes matrices as file and performs different mathmatical operations on them. This is created solely using bash commands so awk and bc, basically anything which would be beneficial for this script is off the table.

### Operations
*Dims:* returns the dimensions of the given matrix.  
*Transpose:* returns the transpose of a given matrix.  
*Mean:* returns a row vector with each element of the vector being the mean of the corresponding column.  
*Add:* returns the matrix created by the addition of two given matrices.  
*Multiply:* returns the product matrix created by multipllying two given matrices.  

### How to Use
Call this program from your terminal followed by the operation you wish to perform and the matrices you wish to perform the operations on.
Default output is to the command line.

### Example Output
```
$ cat m1
1	2	3	4
5	6	7	8
$ cat m2
1	2
3	4
5	6
7	8
$ ./matrix dims m1
2 4
$ cat m2 | ./matrix dims
4 2
$ ./matrix add m1 m1
2	4	6	8
10	12	14	16
$ ./matrix add m2 m2
2	4
6	8
10	12
14	16
$ ./matrix mean m1
3	4	5	6
$ ./matrix transpose m1
1	5
2	6
3	7
4	8
$ ./matrix multiply m1 m2
50	60
114	140
```
### Creation Purpose
This script was created as an assignment for an Operating Systems I class

