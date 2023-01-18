## Description

<div><p>You are given an array $a$ consisting of $n$ positive integers. Find a <span class="tex-font-style-bf">non-empty</span> subset of its elements such that their sum is <span class="tex-font-style-bf">even</span> (i.e. divisible by $2$) or determine that there is no such subset.</p><p>Both the given array and required subset may contain equal values.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 100$), number of test cases to solve. Descriptions of $t$ test cases follow.</p><p>A description of each test case consists of two lines. The first line contains a single integer $n$ ($1 \leq n \leq 100$), length of array $a$.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 100$), elements of $a$. The given array $a$ can contain equal values (duplicates).</p></div><div class="output-specification"><p>For each test case output $-1$ if there is no such subset of elements. Otherwise output positive integer $k$, number of elements in the required subset. Then output $k$ distinct integers ($1 \leq p_i \leq n$), indexes of the chosen elements. If there are multiple solutions output any of them.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 100$), number of test cases to solve. Descriptions of $t$ test cases follow.</p><p>A description of each test case consists of two lines. The first line contains a single integer $n$ ($1 \leq n \leq 100$), length of array $a$.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 100$), elements of $a$. The given array $a$ can contain equal values (duplicates).</p>

## Output

<p>For each test case output $-1$ if there is no such subset of elements. Otherwise output positive integer $k$, number of elements in the required subset. Then output $k$ distinct integers ($1 \leq p_i \leq n$), indexes of the chosen elements. If there are multiple solutions output any of them.</p>





```input1
3
3
1 4 3
1
15
2
3 5
```




```output1
1
2
-1
2
1 2
```



## Note

<p>There are three test cases in the example.</p><p>In the first test case, you can choose the subset consisting of only the second element. Its sum is $4$ and it is even.</p><p>In the second test case, there is only one non-empty subset of elements consisting of the first element, however sum in it is odd, so there is no solution.</p><p>In the third test case, the subset consisting of all array's elements has even sum.</p>
