## Description

<div><p><span class="tex-font-style-bf">This is the hard version of this problem. The difference between easy and hard versions is only the constraints on $a_i$ and on $n$. You can make hacks only if both versions of the problem are solved.</span></p><p>Burenka is the crown princess of Buryatia, and soon she will become the $n$-th queen of the country. There is an ancient tradition in Buryatia&nbsp;— before the coronation, the ruler must show their strength to the inhabitants. To determine the strength of the $n$-th ruler, the inhabitants of the country give them an array of $a$ of exactly $n$ numbers, after which the ruler must turn all the elements of the array into zeros in the shortest time. The ruler can do the following two-step operation any number of times: </p><ul> <li> select two indices $l$ and $r$, so that $1 \le l \le r \le n$ and a non-negative integer $x$, then </li><li> for all $l \leq i \leq r$ assign $a_i := a_i \oplus x$, where $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>. It takes $\left\lceil \frac{r-l+1}{2} \right\rceil$ seconds to do this operation, where $\lceil y \rceil$ denotes $y$ rounded up to the nearest integer. </li></ul><p>Help Burenka calculate how much time she will need.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ $(1 \le t \le 500)$ &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ $(1 \le n \le 10^5)$ - the size of the array</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \cdots , a_n$ $(0 \le a_i &lt; 2^{30})$&nbsp;— elements of the array.</p><p>It is guaranteed that the sum of $n$ in all tests does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, output a single number &nbsp;— the minimum time that Burenka will need.</p></div>

## Input

<p>The first line contains a single integer $t$ $(1 \le t \le 500)$ &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ $(1 \le n \le 10^5)$ - the size of the array</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \cdots , a_n$ $(0 \le a_i &lt; 2^{30})$&nbsp;— elements of the array.</p><p>It is guaranteed that the sum of $n$ in all tests does not exceed $10^5$.</p>

## Output

<p>For each test case, output a single number &nbsp;— the minimum time that Burenka will need.</p>





```input1|2,3,6,7,10,11,14,15
7
4
5 5 5 5
3
1 3 2
2
0 0
3
2 5 7
6
1 2 3 3 2 1
10
27 27 34 32 2 31 23 56 52 4
5
1822 1799 57 23 55
```




```output1
2
2
0
2
4
7
4
```



## Note

<p>In the first test case, Burenka can choose segment $l = 1$, $r = 4$, and $x=5$. so it will fill the array with zeros in $2$ seconds.</p><p>In the second test case, Burenka first selects segment $l = 1$, $r = 2$, and $x = 1$, after which $a = [0, 2, 2]$, and then the segment $l = 2$, $r = 3$, and $x=2$, which fills the array with zeros. In total, Burenka will spend $2$ seconds.</p>
