## Description

<div><p>You are given a binary matrix $A$ of size $n \times n$. Rows are numbered from top to bottom from $1$ to $n$, columns are numbered from left to right from $1$ to $n$. The element located at the intersection of row $i$ and column $j$ is called $A_{ij}$. Consider a set of $4$ operations:</p><ol> <li> Cyclically shift all rows up. The row with index $i$ will be written in place of the row $i-1$ ($2 \le i \le n$), the row with index $1$ will be written in place of the row $n$. </li><li> Cyclically shift all rows down. The row with index $i$ will be written in place of the row $i+1$ ($1 \le i \le n - 1$), the row with index $n$ will be written in place of the row $1$. </li><li> Cyclically shift all columns to the left. The column with index $j$ will be written in place of the column $j-1$ ($2 \le j \le n$), the column with index $1$ will be written in place of the column $n$. </li><li> Cyclically shift all columns to the right. The column with index $j$ will be written in place of the column $j+1$ ($1 \le j \le n - 1$), the column with index $n$ will be written in place of the column $1$. </li></ol><center> <img class="tex-graphics" src="file://quTt2YeY.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">The $3 \times 3$ matrix is shown on the left before the $3$-rd operation is applied to it, on the right&nbsp;— after.</span> </center><p>You can perform an arbitrary (possibly zero) number of operations on the matrix; the operations can be performed in any order.</p><p>After that, you can perform an arbitrary (possibly zero) number of new xor-operations:</p><ul> <li> Select any element $A_{ij}$ and assign it with new value $A_{ij} \oplus 1$. In other words, the value of $(A_{ij} + 1) \bmod 2$ will have to be written into element $A_{ij}$. </li></ul><p>Each application of this xor-operation costs one burl. Note that the $4$ shift operations&nbsp;— are free. These $4$ operations can only be performed before xor-operations are performed.</p><p>Output the minimum number of burles you would have to pay to make the $A$ matrix unitary. A <span class="tex-font-style-it">unitary matrix</span> is a matrix with ones on the main diagonal and the rest of its elements are zeros (that is, $A_{ij} = 1$ if $i = j$ and $A_{ij} = 0$ otherwise).</p></div><div class="input-specification"><p>The first line of the input contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;—the number of test cases in the test.</p><p>The descriptions of the test cases follow. Before each test case, an empty line is written in the input.</p><p>The first line of each test case contains a single number $n$ ($1 \le n \le 2000$)</p><p>This is followed by $n$ lines, each containing exactly $n$ characters and consisting only of zeros and ones. These lines describe the values in the elements of the matrix.</p><p>It is guaranteed that the sum of $n^2$ values over all test cases does not exceed $4 \cdot 10^6$.</p></div><div class="output-specification"><p>For each test case, output the minimum number of burles you would have to pay to make the $A$ matrix unitary. In other words, print the minimum number of xor-operations it will take after applying cyclic shifts to the matrix for the $A$ matrix to become unitary.</p></div>

## Input

<p>The first line of the input contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;—the number of test cases in the test.</p><p>The descriptions of the test cases follow. Before each test case, an empty line is written in the input.</p><p>The first line of each test case contains a single number $n$ ($1 \le n \le 2000$)</p><p>This is followed by $n$ lines, each containing exactly $n$ characters and consisting only of zeros and ones. These lines describe the values in the elements of the matrix.</p><p>It is guaranteed that the sum of $n^2$ values over all test cases does not exceed $4 \cdot 10^6$.</p>

## Output

<p>For each test case, output the minimum number of burles you would have to pay to make the $A$ matrix unitary. In other words, print the minimum number of xor-operations it will take after applying cyclic shifts to the matrix for the $A$ matrix to become unitary.</p>





```input1
4

3
010
011
100

5
00010
00001
10000
01000
00100

2
10
10

4
1111
1011
1111
1111
```




```output1
1
0
2
11
```



## Note

<p>In the first test case, you can do the following: first, shift all the rows down cyclically, then the main diagonal of the matrix will contain only "<span class="tex-font-style-tt">1</span>". Then it will be necessary to apply xor-operation to the only "<span class="tex-font-style-tt">1</span>" that is not on the main diagonal.</p><p>In the second test case, you can make a unitary matrix by applying the operation $2$&nbsp;— cyclic shift of rows upward twice to the matrix.</p>
