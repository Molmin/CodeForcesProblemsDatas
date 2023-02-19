## Description

<div><p>According to a legend the Hanoi Temple holds a permutation of integers from $1$ to $n$. There are $n$ stones of distinct colors lying in one line in front of the temple. Monks can perform the following operation on stones: choose a position $i$ ($1 \le i \le n$) and cyclically shift stones at positions $i$, $p[i]$, $p[p[i]]$, .... That is, a stone from position $i$ will move to position $p[i]$, a stone from position $p[i]$ will move to position $p[p[i]]$, and so on, a stone from position $j$, such that $p[j] = i$, will move to position $i$.</p><p>Each day the monks must obtain a new arrangement of stones using an arbitrary number of these operations. When all possible arrangements will have been obtained, the world will end. You are wondering, what if some elements of the permutation could be swapped just before the beginning? How many days would the world last?</p><p>You want to get a permutation that will allow the world to last as long as possible, using the minimum number of exchanges of two elements of the permutation.</p><p>Two arrangements of stones are considered different if there exists a position $i$ such that the colors of the stones on that position are different in these arrangements.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 10^3$). Description of the test cases follows.</p><p>The first line of each test case contains $n$ ($3 \leq n \leq 10^6$). The next line contains $n$ integers $p_1, \dots, p_n$ ($1 \le p_i \le n$). It is guaranteed that $p$ is a permutation.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$. </p></div><div class="output-specification"><p>For each of the $t$ test cases, print two integers on a new line: the largest possible number of days the world can last, modulo $10^9 + 7$, and the minimum number of exchanges required for that.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 10^3$). Description of the test cases follows.</p><p>The first line of each test case contains $n$ ($3 \leq n \leq 10^6$). The next line contains $n$ integers $p_1, \dots, p_n$ ($1 \le p_i \le n$). It is guaranteed that $p$ is a permutation.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$. </p>

## Output

<p>For each of the $t$ test cases, print two integers on a new line: the largest possible number of days the world can last, modulo $10^9 + 7$, and the minimum number of exchanges required for that.</p>





```input1
3
3
2 3 1
3
2 1 3
3
1 2 3
```




```input2
5
4
2 3 4 1
4
2 3 1 4
4
2 1 4 3
4
2 1 3 4
4
1 2 3 4
```




```output1
3 0
3 1
3 2
```




```output2
4 0
4 1
4 0
4 1
4 2
```



## Note

<p>Let's label the colors of the stones with letters. Explanations for the first two test cases of the first example: </p><ol> <li> Using the permutation $[2, 3, 1]$, we can additionally obtain the arrangements <span class="tex-font-style-tt">CAB</span> and <span class="tex-font-style-tt">BCA</span> from <span class="tex-font-style-tt">ABC</span>. This is already the maximum possible result. </li><li> Using the permutation $[2, 1, 3]$, the only <span class="tex-font-style-tt">BAC</span> can be obtained from <span class="tex-font-style-tt">ABC</span>. As we saw in the previous case, two arrangements are not the maximum possible number of distinct arrangements for $n = 3$. To get an optimal permutation, for example, we can swap $1$ and $3$, so we will get the permutation $[2, 3, 1]$. </li></ol>
