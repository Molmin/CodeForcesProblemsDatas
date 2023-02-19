## Description

<div><p>A sequence of $n$ numbers is called <span class="tex-font-style-it">permutation</span> if it contains all integers from $1$ to $n$ exactly once. For example, the sequences [$3, 1, 4, 2$], [$1$] and [$2,1$] are permutations, but [$1,2,1$], [$0,1$] and [$1,3,4$]&nbsp;— are not.</p><p>Kristina had a permutation $p$ of $n$ elements. She wrote it on the whiteboard $n$ times in such a way that: </p><ul> <li> while writing the permutation at the $i$-th ($1 \le i \le n)$ time she skipped the element $p_i$ </li></ul> So, she wrote in total $n$ sequences of length $n-1$ each.<p>For example, suppose Kristina had a permutation $p$ = $[4,2,1,3]$ of length $4$. Then she did the following: </p><ol> <li> Wrote the sequence $[2, 1, 3]$, skipping the element $p_1=4$ from the original permutation. </li><li> Wrote the sequence $[4, 1, 3]$, skipping the element $p_2=2$ from the original permutation. </li><li> Wrote the sequence $[4, 2, 3]$, skipping the element $p_3=1$ from the original permutation. </li><li> Wrote the sequence $[4, 2, 1]$, skipping the element $p_4=3$ from the original permutation. </li></ol><p>You know all $n$ of sequences that have been written on the whiteboard, but you do not know the order in which they were written. They are given in <span class="tex-font-style-bf">arbitrary order</span>. Reconstruct the original permutation from them.</p><p>For example, if you know the sequences $[4, 2, 1]$, $[4, 2, 3]$, $[2, 1, 3]$, $[4, 1, 3]$, then the original permutation will be $p$ = $[4, 2, 1, 3]$.</p></div><div class="input-specification"><p>The first line of input data contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The description of the test cases follows.</p><p>The first line of each test case contains one integer $n$ ($3 \le n \le 100$).</p><p>This is followed by $n$ lines, each containing exactly $n-1$ integers and describing one of the sequences written out on the whiteboard.</p><p>It is guaranteed that all sequences could be obtained from some permutation $p$, and that the sum $n^2$ over all input sets does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output on a separate line a permutation $p$ such that the given $n$ sequences could be obtained from it.</p><p>It is guaranteed that the answer exists and it is the only one. In other words, for each test case the required permutation is sure to exist.</p></div>

## Input

<p>The first line of input data contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The description of the test cases follows.</p><p>The first line of each test case contains one integer $n$ ($3 \le n \le 100$).</p><p>This is followed by $n$ lines, each containing exactly $n-1$ integers and describing one of the sequences written out on the whiteboard.</p><p>It is guaranteed that all sequences could be obtained from some permutation $p$, and that the sum $n^2$ over all input sets does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output on a separate line a permutation $p$ such that the given $n$ sequences could be obtained from it.</p><p>It is guaranteed that the answer exists and it is the only one. In other words, for each test case the required permutation is sure to exist.</p>





```input1|2,3,4,5,6,11,12,13,14,15,16,22,23,24,25
5
4
4 2 1
4 2 3
2 1 3
4 1 3
3
2 3
1 3
1 2
5
4 2 1 3
2 1 3 5
4 2 3 5
4 1 3 5
4 2 1 5
4
2 3 4
1 3 4
1 2 3
1 2 4
3
2 1
1 3
2 3
```




```output1
4 2 1 3 
1 2 3 
4 2 1 3 5 
1 2 3 4 
2 1 3
```



## Note

<p>The first test case is described in the problem statement.</p><p>In the second test case, the sequences are written in the correct order.</p>
