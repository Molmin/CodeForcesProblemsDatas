## Description

<div><p>There is a street with $n$ houses in a line, numbered from $1$ to $n$. The house $i$ is initially painted in color $c_i$. The street is considered beautiful if all houses are painted in the same color. Tom, the painter, is in charge of making the street beautiful. Tom's painting capacity is defined by an integer, let's call it $k$.</p><p>On one day, Tom can do the following repainting process that consists of two steps: </p><ol> <li> He chooses two integers $l$ and $r$ such that $ 1 \le l \le r \le n $ and $ r - l + 1 = k $. </li><li> For each house $i$ such that $l \le i \le r$, he can either repaint it with any color he wants, or ignore it and let it keep its current color. </li></ol><p>Note that in the same day Tom can use different colors to repaint different houses.</p><p>Tom wants to know the minimum number of days needed to repaint the street so that it becomes beautiful.</p></div><div class="input-specification"><p>The first line of input contains a single integer $t$ ($ 1 \le t \le 10^4$), the number of test cases. Description of test cases follows.</p><p>In the first line of a test case description there are two integers $n$ and $k$ ($1 \le k \le n \le 10^5$).</p><p>The second line contains $n$ space-separated integers. The $i$-th of these integers represents $c_i$ ($1 \le c_i \le 100$), the color which house $i$ is initially painted in.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>Print $t$ lines, each with one integer: the minimum number of days Tom needs to make the street beautiful for each test case. </p></div>

## Input

<p>The first line of input contains a single integer $t$ ($ 1 \le t \le 10^4$), the number of test cases. Description of test cases follows.</p><p>In the first line of a test case description there are two integers $n$ and $k$ ($1 \le k \le n \le 10^5$).</p><p>The second line contains $n$ space-separated integers. The $i$-th of these integers represents $c_i$ ($1 \le c_i \le 100$), the color which house $i$ is initially painted in.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>Print $t$ lines, each with one integer: the minimum number of days Tom needs to make the street beautiful for each test case. </p>





```input1
3
10 2
1 1 2 2 1 1 2 2 2 1
7 1
1 2 3 4 5 6 7
10 3
1 3 3 3 3 1 2 1 3 3
```




```output1
3
6
2
```



## Note

<p>In the first test case Tom should paint houses 1 and 2 in the first day in color 2, houses 5 and 6 in the second day in color 2, and the last house in color 2 on the third day.</p><p>In the second test case Tom can, for example, spend 6 days to paint houses 1, 2, 4, 5, 6, 7 in color 3.</p><p>In the third test case Tom can paint the first house in the first day and houses 6, 7, and 8 in the second day in color 3.</p>
