## Description

<div><p>You are given an array $a[0 \dots n-1]$ of $n$ integers. This array is called a "<span class="tex-font-style-it">valley</span>" if there exists <span class="tex-font-style-bf">exactly one</span> subarray $a[l \dots r]$ such that:</p><ul> <li> $0 \le l \le r \le n-1$, </li><li> $a_l = a_{l+1} = a_{l+2} = \dots = a_r$, </li><li> $l = 0$ or $a_{l-1} &gt; a_{l}$, </li><li> $r = n-1$ or $a_r &lt; a_{r+1}$. </li></ul><p>Here are three examples:</p><center> <img class="tex-graphics" src="file://Of8e0qAH.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The first image shows the array [$3, 2, 2, 1, 2, 2, 3$], it <span class="tex-font-style-bf">is a valley</span> because only subarray with indices $l=r=3$ satisfies the condition.</p><p>The second image shows the array [$1, 1, 1, 2, 3, 3, 4, 5, 6, 6, 6$], it <span class="tex-font-style-bf">is a valley</span> because only subarray with indices $l=0, r=2$ satisfies the codition.</p><p>The third image shows the array [$1, 2, 3, 4, 3, 2, 1$], it <span class="tex-font-style-bf">is not a valley</span> because two subarrays $l=r=0$ and $l=r=6$ that satisfy the condition.</p><p>You are asked whether the given array is a valley or not.</p><p><span class="tex-font-style-it">Note that we consider the array to be indexed from $0$.</span></p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 2\cdot10^5$)&nbsp;— the length of the array.</p><p>The second line of each test case contains $n$ integers $a_i$ ($1 \leq a_i \leq 10^9$)&nbsp;— the elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases is smaller than $2\cdot10^5$.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">YES</span>" (without quotes) if the array is a valley, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output the answer in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 2\cdot10^5$)&nbsp;— the length of the array.</p><p>The second line of each test case contains $n$ integers $a_i$ ($1 \leq a_i \leq 10^9$)&nbsp;— the elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases is smaller than $2\cdot10^5$.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">YES</span>" (without quotes) if the array is a valley, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output the answer in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p>





```input1|2,3,6,7,10,11
6
7
3 2 2 1 2 2 3
11
1 1 1 2 3 3 4 5 6 6 6
7
1 2 3 4 3 2 1
7
9 7 4 6 9 9 10
1
1000000000
8
9 4 4 5 9 4 9 10
```




```output1
YES
YES
NO
YES
YES
NO
```



## Note

<p>The first three test cases are explained in the statement.</p>
