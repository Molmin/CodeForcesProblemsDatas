## Description

<div><p>Let's define $f(x)$ for a positive integer $x$ as the length of the base-10 representation of $x$ without leading zeros. I like to call it a digital logarithm. Similar to a digital root, if you are familiar with that.</p><p>You are given two arrays $a$ and $b$, each containing $n$ positive integers. In one operation, you do the following: </p><ol> <li> pick some integer $i$ from $1$ to $n$; </li><li> assign either $f(a_i)$ to $a_i$ or $f(b_i)$ to $b_i$. </li></ol><p>Two arrays are considered similar to each other if you can rearrange the elements in both of them, so that they are equal (e. g. $a_i = b_i$ for all $i$ from $1$ to $n$).</p><p>What's the smallest number of operations required to make $a$ and $b$ similar to each other?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of the testcase contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the number of elements in each of the arrays.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i &lt; 10^9$).</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_j &lt; 10^9$).</p><p>The sum of $n$ over all testcases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each testcase, print the smallest number of operations required to make $a$ and $b$ similar to each other.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of the testcase contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the number of elements in each of the arrays.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i &lt; 10^9$).</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_j &lt; 10^9$).</p><p>The sum of $n$ over all testcases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each testcase, print the smallest number of operations required to make $a$ and $b$ similar to each other.</p>





```input1|2,3,4,8,9,10
4
1
1
1000
4
1 2 3 4
3 1 4 2
3
2 9 3
1 100 9
10
75019 709259 5 611271314 9024533 81871864 9 3 6 4865
9503 2 371245467 6 7 37376159 8 364036498 52295554 169
```




```output1
2
0
2
18
```



## Note

<p>In the first testcase, you can apply the digital logarithm to $b_1$ twice.</p><p>In the second testcase, the arrays are already similar to each other.</p><p>In the third testcase, you can first apply the digital logarithm to $a_1$, then to $b_2$.</p>
