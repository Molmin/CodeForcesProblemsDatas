## Description

<div><p>Your friend has created a nearest point function. For a given array of integer points $x$ (<span class="tex-font-style-bf">sorted</span> in ascending order, without any duplicates) and a point $y$ it can find the nearest point from $x$ to the point $y$. In other words, it will find such a point $x_i$ that $|y - x_i|$ is the minimum possible, where $|a|$ is the absolute value of $a$.</p><p>For example, if $x = [1, 2, 5, 7, 9, 11]$, the answer for $y=3$ will be $2$, the answer for $y=5$ will be $5$ and the answer for $y=100$ will be $11$.</p><p>This function is a bit buggy, though. If there are several nearest points to the given one, the function crashes. For example, if $x = [1, 2, 5, 7, 9, 11]$ (as above) and $y=6$, the function will crash, since points $5$ and $7$ are both the nearest points for $6$.</p><p>Your task is, for a given array of integer points $x$ (<span class="tex-font-style-bf">sorted</span> in ascending order, without any duplicates), determine if it is possible to cause the function to crash by choosing some <span class="tex-font-style-bf">integer</span> point $y$.</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>The first line of the test case contains one integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the number of points in the array $x$.</p><p>The second line of the test case contains $n$ integers $x_1, x_2, \ldots, x_n$ ($1 \le x_i \le 10^9$), where $x_i$ is the $i$-th point in the array $x$.</p><p>All points in the array $x$ are distinct, and the array $x$ is sorted in ascending order (in other words, $x_1 &lt; x_2 &lt; \ldots &lt; x_n$).</p><p>The sum of $n$ over the test cases in the input does not exceed $2 \cdot 10^5$ ($\sum n \le 2 \cdot 10^5$).</p></div><div class="output-specification"><p>For each test case, print <span class="tex-font-style-tt">YES</span> if it is possible to find some <span class="tex-font-style-bf">integer</span> point $y$ that will crash the function and <span class="tex-font-style-tt">NO</span> otherwise.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>The first line of the test case contains one integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the number of points in the array $x$.</p><p>The second line of the test case contains $n$ integers $x_1, x_2, \ldots, x_n$ ($1 \le x_i \le 10^9$), where $x_i$ is the $i$-th point in the array $x$.</p><p>All points in the array $x$ are distinct, and the array $x$ is sorted in ascending order (in other words, $x_1 &lt; x_2 &lt; \ldots &lt; x_n$).</p><p>The sum of $n$ over the test cases in the input does not exceed $2 \cdot 10^5$ ($\sum n \le 2 \cdot 10^5$).</p>

## Output

<p>For each test case, print <span class="tex-font-style-tt">YES</span> if it is possible to find some <span class="tex-font-style-bf">integer</span> point $y$ that will crash the function and <span class="tex-font-style-tt">NO</span> otherwise.</p>





```input1
7
2
1 3
2
1 100
3
1 50 101
2
1 1000000000
2
1 999999999
6
1 2 5 7 9 11
6
1 2 5 8 9 12
```




```output1
YES
NO
NO
NO
YES
YES
NO
```



## Note

<p>In the first test case of the example, the function crashes if $y = 2$ is chosen.</p><p>In the fifth test case of the example, the function crashes if $y = 500000000$ is chosen.</p><p>In the sixth test case of the example, the function crashes if $y = 10$ is chosen.</p>
