## Description

<div><p>Monocarp wrote down two numbers on a whiteboard. Both numbers follow a specific format: a positive integer $x$ with $p$ zeros appended to its end.</p><p>Now Monocarp asks you to compare these two numbers. Can you help him?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains two integers $x_1$ and $p_1$ ($1 \le x_1 \le 10^6; 0 \le p_1 \le 10^6$)&nbsp;— the description of the first number.</p><p>The second line of each testcase contains two integers $x_2$ and $p_2$ ($1 \le x_2 \le 10^6; 0 \le p_2 \le 10^6$)&nbsp;— the description of the second number.</p></div><div class="output-specification"><p>For each testcase print the result of the comparison of the given two numbers. If the first number is smaller than the second one, print '&lt;'. If the first number is greater than the second one, print '&gt;'. If they are equal, print '='.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains two integers $x_1$ and $p_1$ ($1 \le x_1 \le 10^6; 0 \le p_1 \le 10^6$)&nbsp;— the description of the first number.</p><p>The second line of each testcase contains two integers $x_2$ and $p_2$ ($1 \le x_2 \le 10^6; 0 \le p_2 \le 10^6$)&nbsp;— the description of the second number.</p>

## Output

<p>For each testcase print the result of the comparison of the given two numbers. If the first number is smaller than the second one, print '&lt;'. If the first number is greater than the second one, print '&gt;'. If they are equal, print '='.</p>





```input1
5
2 1
19 0
10 2
100 1
1999 0
2 3
1 0
1 0
99 0
1 2
```




```output1
&gt;
=
&lt;
=
&lt;
```



## Note

<p>The comparisons in the example are: $20 &gt; 19$, $1000 = 1000$, $1999 &lt; 2000$, $1 = 1$, $99 &lt; 100$.</p>
