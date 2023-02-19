## Description

<div><p>A sequence of $n$ numbers is called <span class="tex-font-style-it">permutation</span> if it contains all numbers from $1$ to $n$ exactly once. For example, the sequences $[3, 1, 4, 2]$, [$1$] and $[2,1]$ are permutations, but $[1,2,1]$, $[0,1]$ and $[1,3,4]$ are not.</p><p>For a given number $n$ you need to make a permutation $p$ such that two requirements are satisfied at the same time:</p><ul> <li> For each element $p_i$, at least one of its neighbors has a value that differs from the value of $p_i$ by one. That is, for each element $p_i$ ($1 \le i \le n$), at least one of its neighboring elements (standing to the left or right of $p_i$) must be $p_i + 1$, or $p_i - 1$. </li><li> the permutation must have no fixed points. That is, for every $i$ ($1 \le i \le n$), $p_i \neq i$ must be satisfied. </li></ul><p>Let's call the permutation that satisfies these requirements <span class="tex-font-style-it">funny</span>.</p><p>For example, let $n = 4$. Then [$4, 3, 1, 2$] is a <span class="tex-font-style-it">funny</span> permutation, since: </p><ul> <li> to the right of $p_1=4$ is $p_2=p_1-1=4-1=3$; </li><li> to the left of $p_2=3$ is $p_1=p_2+1=3+1=4$; </li><li> to the right of $p_3=1$ is $p_4=p_3+1=1+1=2$; </li><li> to the left of $p_4=2$ is $p_3=p_4-1=2-1=1$. </li><li> for all $i$ is $p_i \ne i$. </li></ul><p>For a given positive integer $n$, output <span class="tex-font-style-bf">any</span> <span class="tex-font-style-it">funny</span> permutation of length $n$, or output <span class="tex-font-style-tt">-1</span> if <span class="tex-font-style-it">funny</span> permutation of length $n$ does not exist.</p></div><div class="input-specification"><p>The first line of input data contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The description of the test cases follows.</p><p>Each test case consists of f single line containing one integer $n$ ($2 \le n \le 2 \cdot 10^5$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print on a separate line: </p><ul> <li> <span class="tex-font-style-bf">any</span> <span class="tex-font-style-it">funny</span> permutation $p$ of length $n$; </li><li> or the number <span class="tex-font-style-tt">-1</span> if the permutation you are looking for does not exist. </li></ul></div>

## Input

<p>The first line of input data contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The description of the test cases follows.</p><p>Each test case consists of f single line containing one integer $n$ ($2 \le n \le 2 \cdot 10^5$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print on a separate line: </p><ul> <li> <span class="tex-font-style-bf">any</span> <span class="tex-font-style-it">funny</span> permutation $p$ of length $n$; </li><li> or the number <span class="tex-font-style-tt">-1</span> if the permutation you are looking for does not exist. </li></ul>





```input1|2,4,6
5
4
3
7
5
2
```




```output1
3 4 2 1
-1
6 7 4 5 3 2 1
5 4 1 2 3
2 1
```



## Note

<p>The first test case is explained in the problem statement.</p><p>In the second test case, it is not possible to make the required permutation: permutations $[1, 2, 3]$, $[1, 3, 2]$, $[2, 1, 3]$, $[3, 2, 1]$ have fixed points, and in $[2, 3, 1]$ and $[3, 1, 2]$ the first condition is met not for all positions.</p>
