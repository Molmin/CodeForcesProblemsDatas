## Description

<div><p>Vasya has written some permutation $p_1, p_2, \ldots, p_n$ of integers from $1$ to $n$, so for all $1 \leq i \leq n$ it is true that $1 \leq p_i \leq n$ and all $p_1, p_2, \ldots, p_n$ are different. After that he wrote $n$ numbers $next_1, next_2, \ldots, next_n$. The number $next_i$ is equal to the minimal index $i &lt; j \leq n$, such that $p_j &gt; p_i$. If there is no such $j$ let's let's define as $next_i = n + 1$.</p><p>In the evening Vasya went home from school and due to rain, his notebook got wet. Now it is impossible to read some written numbers. Permutation and some values $next_i$ are completely lost! If for some $i$ the value $next_i$ is lost, let's say that $next_i = -1$.</p><p>You are given numbers $next_1, next_2, \ldots, next_n$ (maybe some of them are equal to $-1$). Help Vasya to find such permutation $p_1, p_2, \ldots, p_n$ of integers from $1$ to $n$, that he can write it to the notebook and all numbers $next_i$, which are not equal to $-1$, will be correct. </p></div><div class="input-specification"><p>The first line contains one integer $t$&nbsp;— the number of test cases ($1 \leq t \leq 100\,000$).</p><p>Next $2 \cdot t$ lines contains the description of test cases,two lines for each. The first line contains one integer $n$&nbsp;— the length of the permutation, written by Vasya ($1 \leq n \leq 500\,000$). The second line contains $n$ integers $next_1, next_2, \ldots, next_n$, separated by spaces ($next_i = -1$ or $i &lt; next_i \leq n + 1$).</p><p>It is guaranteed, that the sum of $n$ in all test cases doesn't exceed $500\,000$.</p><p>In <span class="tex-font-style-bf">hacks</span> you can only use one test case, so $T = 1$.</p></div><div class="output-specification"><p>Print $T$ lines, in $i$-th of them answer to the $i$-th test case.</p><p>If there is no such permutations $p_1, p_2, \ldots, p_n$ of integers from $1$ to $n$, that Vasya could write, print the only number $-1$.</p><p>In the other case print $n$ different integers $p_1, p_2, \ldots, p_n$, separated by spaces ($1 \leq p_i \leq n$). All defined values of $next_i$ which are not equal to $-1$ should be computed correctly $p_1, p_2, \ldots, p_n$ using defenition given in the statement of the problem. If there exists more than one solution you can find any of them.</p></div>

## Input

<p>The first line contains one integer $t$&nbsp;— the number of test cases ($1 \leq t \leq 100\,000$).</p><p>Next $2 \cdot t$ lines contains the description of test cases,two lines for each. The first line contains one integer $n$&nbsp;— the length of the permutation, written by Vasya ($1 \leq n \leq 500\,000$). The second line contains $n$ integers $next_1, next_2, \ldots, next_n$, separated by spaces ($next_i = -1$ or $i &lt; next_i \leq n + 1$).</p><p>It is guaranteed, that the sum of $n$ in all test cases doesn't exceed $500\,000$.</p><p>In <span class="tex-font-style-bf">hacks</span> you can only use one test case, so $T = 1$.</p>

## Output

<p>Print $T$ lines, in $i$-th of them answer to the $i$-th test case.</p><p>If there is no such permutations $p_1, p_2, \ldots, p_n$ of integers from $1$ to $n$, that Vasya could write, print the only number $-1$.</p><p>In the other case print $n$ different integers $p_1, p_2, \ldots, p_n$, separated by spaces ($1 \leq p_i \leq n$). All defined values of $next_i$ which are not equal to $-1$ should be computed correctly $p_1, p_2, \ldots, p_n$ using defenition given in the statement of the problem. If there exists more than one solution you can find any of them.</p>





```input1
6
3
2 3 4
2
3 3
3
-1 -1 -1
3
3 4 -1
1
2
4
4 -1 4 5
```




```output1
1 2 3
2 1
2 1 3
-1
1
3 2 1 4
```



## Note

<p>In the first test case for permutation $p = [1, 2, 3]$ Vasya should write $next = [2, 3, 4]$, because each number in permutation is less than next. It's easy to see, that it is the only satisfying permutation.</p><p>In the third test case, any permutation can be the answer because all numbers $next_i$ are lost.</p><p>In the fourth test case, there is no satisfying permutation, so the answer is $-1$.</p>
