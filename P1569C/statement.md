## Description

<div><p>$n$ people gathered to hold a jury meeting of the upcoming competition, the $i$-th member of the jury came up with $a_i$ tasks, which they want to share with each other.</p><p>First, the jury decides on the order which they will follow while describing the tasks. Let that be a permutation $p$ of numbers from $1$ to $n$ (an array of size $n$ where each integer from $1$ to $n$ occurs exactly once).</p><p>Then the discussion goes as follows:</p><ul> <li> If a jury member $p_1$ has some tasks left to tell, then they tell one task to others. Otherwise, they are skipped. </li><li> If a jury member $p_2$ has some tasks left to tell, then they tell one task to others. Otherwise, they are skipped. </li><li> ... </li><li> If a jury member $p_n$ has some tasks left to tell, then they tell one task to others. Otherwise, they are skipped. </li><li> If there are still members with tasks left, then the process repeats from the start. Otherwise, the discussion ends. </li></ul><p>A permutation $p$ is nice if none of the jury members tell two or more of their own tasks in a row. </p><p>Count the number of nice permutations. The answer may be really large, so print it modulo $998\,244\,353$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of the test case contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$)&nbsp;— number of jury members.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the number of problems that the $i$-th member of the jury came up with.</p><p>The sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print one integer&nbsp;— the number of nice permutations, taken modulo $998\,244\,353$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of the test case contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$)&nbsp;— number of jury members.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the number of problems that the $i$-th member of the jury came up with.</p><p>The sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print one integer&nbsp;— the number of nice permutations, taken modulo $998\,244\,353$.</p>





```input1
4
2
1 2
3
5 5 5
4
1 3 3 7
6
3 4 2 1 3 3
```




```output1
1
6
0
540
```



## Note

<p>Explanation of the first test case from the example:</p><p>There are two possible permutations, $p = [1, 2]$ and $p = [2, 1]$. For $p = [1, 2]$, the process is the following:</p><ol> <li> the first jury member tells a task; </li><li> the second jury member tells a task; </li><li> the first jury member doesn't have any tasks left to tell, so they are skipped; </li><li> the second jury member tells a task. </li></ol><p>So, the second jury member has told two tasks in a row (in succession), so the permutation is not nice.</p><p>For $p = [2, 1]$, the process is the following:</p><ol> <li> the second jury member tells a task; </li><li> the first jury member tells a task; </li><li> the second jury member tells a task. </li></ol><p>So, this permutation is nice.</p>
