## Description

<div><p>You are given a set of size $m$ with integer elements between $0$ and $2^{n}-1$ inclusive. Let's build an undirected graph on these integers in the following way: connect two integers $x$ and $y$ with an edge if and only if $x \&amp; y = 0$. Here $\&amp;$ is the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#AND">bitwise AND operation</a>. Count the number of connected components in that graph.</p></div><div class="input-specification"><p>In the first line of input there are two integers $n$ and $m$ ($0 \le n \le 22$, $1 \le m \le 2^{n}$).</p><p>In the second line there are $m$ integers $a_1, a_2, \ldots, a_m$ ($0 \le a_{i} &lt; 2^{n}$)&nbsp;— the elements of the set. All $a_{i}$ are distinct.</p></div><div class="output-specification"><p>Print the number of connected components.</p></div>

## Input

<p>In the first line of input there are two integers $n$ and $m$ ($0 \le n \le 22$, $1 \le m \le 2^{n}$).</p><p>In the second line there are $m$ integers $a_1, a_2, \ldots, a_m$ ($0 \le a_{i} &lt; 2^{n}$)&nbsp;— the elements of the set. All $a_{i}$ are distinct.</p>

## Output

<p>Print the number of connected components.</p>





```input1
2 3
1 2 3

```




```input2
5 5
5 19 10 20 12

```




```output1
2

```




```output2
2

```



## Note

<p>Graph from first sample:</p><p><img class="tex-graphics" src="file://0IwKCzJf.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Graph from second sample:</p><p><img class="tex-graphics" src="file://1kd50dYf.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
