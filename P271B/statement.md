## Description

<div><p>You've got an <span class="tex-span"><i>n</i> × <i>m</i></span> matrix. The matrix consists of integers. In one move, you can apply a single transformation to the matrix: choose an arbitrary element of the matrix and increase it by <span class="tex-span">1</span>. Each element can be increased an arbitrary number of times.</p><p>You are really curious about prime numbers. Let us remind you that a <span class="tex-font-style-it">prime number</span> is a positive integer that has exactly two distinct positive integer divisors: itself and number one. For example, numbers 2, 3, 5 are prime and numbers 1, 4, 6 are not. </p><p>A matrix is <span class="tex-font-style-it">prime</span> if at least one of the two following conditions fulfills:</p><ul> <li> the matrix has a row with prime numbers only; </li><li> the matrix has a column with prime numbers only; </li></ul><p>Your task is to count the minimum number of moves needed to get a prime matrix from the one you've got.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 500)</span> — the number of rows and columns in the matrix, correspondingly.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> integers — the initial matrix. All matrix elements are positive integers. All numbers in the initial matrix do not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p><p>The numbers in the lines are separated by single spaces.</p></div><div class="output-specification"><p>Print a single integer — the minimum number of moves needed to get a prime matrix from the one you've got. If you've got a prime matrix, print 0.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 500)</span> — the number of rows and columns in the matrix, correspondingly.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> integers — the initial matrix. All matrix elements are positive integers. All numbers in the initial matrix do not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p><p>The numbers in the lines are separated by single spaces.</p>

## Output

<p>Print a single integer — the minimum number of moves needed to get a prime matrix from the one you've got. If you've got a prime matrix, print 0.</p>





```input1
3 3
1 2 3
5 6 1
4 4 1

```




```input2
2 3
4 8 8
9 2 9

```




```input3
2 2
1 3
4 2

```




```output1
1

```




```output2
3

```




```output3
0

```



## Note

<p>In the first sample you need to increase number 1 in cell (1, 1). Thus, the first row will consist of prime numbers: 2, 2, 3.</p><p>In the second sample you need to increase number 8 in cell (1, 2) three times. Thus, the second column will consist of prime numbers: 11, 2.</p><p>In the third sample you don't have to do anything as the second column already consists of prime numbers: 3, 2. </p>
