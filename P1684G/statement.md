## Description

<div><p>Let's consider Euclid's algorithm for finding the <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor</a>, where $t$ is a list:</p><pre class="verbatim"><br>function Euclid(a, b):<br>    if a &lt; b:<br>        swap(a, b)<br><br>    if b == 0:<br>        return a<br><br>    r = reminder from dividing a by b<br>    if r &gt; 0:<br>        append r to the back of t<br><br>    return Euclid(b, r)<br></pre><p>There is an array $p$ of pairs of positive integers that are not greater than $m$. Initially, the list $t$ is empty. Then the function is run on each pair in $p$. After that the list $t$ is shuffled and given to you.</p><p>You have to find an array $p$ <span class="tex-font-style-bf">of any size</span> not greater than $2 \cdot 10^4$ that produces the given list $t$, or tell that no such array exists.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n \le 10^3$, $1 \le m \le 10^9$)&nbsp;— the length of the array $t$ and the constraint for integers in pairs.</p><p>The second line contains $n$ integers $t_1, t_2, \ldots, t_n$ ($1 \le t_i \le m$)&nbsp;— the elements of the array $t$.</p></div><div class="output-specification"><ul> <li> If the answer does not exist, output $-1$. </li><li> If the answer exists, in the first line output $k$ ($1 \le k \le 2 \cdot 10^4$)&nbsp;— the size of your array $p$, i.&nbsp;e. the number of pairs in the answer. <p>The $i$-th of the next $k$ lines should contain two integers $a_i$ and $b_i$ ($1 \le a_i, b_i \le m$)&nbsp;— the $i$-th pair in $p$.</p></li></ul><p>If there are multiple valid answers you can output any of them.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n \le 10^3$, $1 \le m \le 10^9$)&nbsp;— the length of the array $t$ and the constraint for integers in pairs.</p><p>The second line contains $n$ integers $t_1, t_2, \ldots, t_n$ ($1 \le t_i \le m$)&nbsp;— the elements of the array $t$.</p>

## Output

<ul> <li> If the answer does not exist, output $-1$. </li><li> If the answer exists, in the first line output $k$ ($1 \le k \le 2 \cdot 10^4$)&nbsp;— the size of your array $p$, i.&nbsp;e. the number of pairs in the answer. <p>The $i$-th of the next $k$ lines should contain two integers $a_i$ and $b_i$ ($1 \le a_i, b_i \le m$)&nbsp;— the $i$-th pair in $p$.</p></li></ul><p>If there are multiple valid answers you can output any of them.</p>





```input1
7 20
1 8 1 6 3 2 3
```




```input2
2 10
7 1
```




```input3
2 15
1 7
```




```input4
1 1000000000
845063470
```




```output1
3
19 11
15 9
3 7
```




```output2
-1
```




```output3
1
15 8
```




```output4
-1
```



## Note

<p>In the first sample let's consider the array $t$ for each pair: </p><ul> <li> $(19,\, 11)$: $t = [8, 3, 2, 1]$; </li><li> $(15,\, 9)$: $t = [6, 3]$; </li><li> $(3,\, 7)$: $t = [1]$. </li></ul><p>So in total $t = [8, 3, 2, 1, 6, 3, 1]$, which is the same as the input $t$ (up to a permutation).</p><p>In the second test case it is impossible to find such array $p$ of pairs that all integers are not greater than $10$ and $t = [7, 1]$</p><p>In the third test case for the pair $(15,\, 8)$ array $t$ will be $[7, 1]$.</p>
