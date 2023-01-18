## Description

<div><p>Alice's hair is growing by leaps and bounds. Maybe the cause of it is the excess of vitamins, or maybe it is some black magic...</p><p>To prevent this, Alice decided to go to the hairdresser. She wants for her hair length to be at most $l$ centimeters after haircut, where $l$ is her favorite number. Suppose, that the Alice's head is a straight line on which $n$ hairlines grow. Let's number them from $1$ to $n$. With one swing of the scissors the hairdresser can shorten all hairlines on any segment to the length $l$, given that <span class="tex-font-style-bf">all</span> hairlines on that segment had length <span class="tex-font-style-bf">strictly greater</span> than $l$. The hairdresser wants to complete his job as fast as possible, so he will make the least possible number of swings of scissors, since each swing of scissors takes one second.</p><p>Alice hasn't decided yet when she would go to the hairdresser, so she asked you to calculate how much time the haircut would take depending on the time she would go to the hairdresser. In particular, you need to process queries of two types:</p><ul> <li> $0$&nbsp;— Alice asks how much time the haircut would take if she would go to the hairdresser now. </li><li> $1$ $p$ $d$&nbsp;— $p$-th hairline grows by $d$ centimeters. </li></ul><p>Note, that in the request $0$ Alice is interested in hypothetical scenario of taking a haircut now, so no hairlines change their length.</p></div><div class="input-specification"><p>The first line contains three integers $n$, $m$ and $l$ ($1 \le n, m \le 100\,000$, $1 \le l \le 10^9$)&nbsp;— the number of hairlines, the number of requests and the favorite number of Alice.</p><p>The second line contains $n$ integers $a_i$ ($1 \le a_i \le 10^9$)&nbsp;— the initial lengths of all hairlines of Alice.</p><p>Each of the following $m$ lines contains a request in the format described in the statement.</p><p>The request description starts with an integer $t_i$. If $t_i = 0$, then you need to find the time the haircut would take. Otherwise, $t_i = 1$ and in this moment one hairline grows. The rest of the line than contains two more integers: $p_i$ and $d_i$ ($1 \le p_i \le n$, $1 \le d_i \le 10^9$)&nbsp;— the number of the hairline and the length it grows by.</p></div><div class="output-specification"><p>For each query of type $0$ print the time the haircut would take.</p></div>

## Input

<p>The first line contains three integers $n$, $m$ and $l$ ($1 \le n, m \le 100\,000$, $1 \le l \le 10^9$)&nbsp;— the number of hairlines, the number of requests and the favorite number of Alice.</p><p>The second line contains $n$ integers $a_i$ ($1 \le a_i \le 10^9$)&nbsp;— the initial lengths of all hairlines of Alice.</p><p>Each of the following $m$ lines contains a request in the format described in the statement.</p><p>The request description starts with an integer $t_i$. If $t_i = 0$, then you need to find the time the haircut would take. Otherwise, $t_i = 1$ and in this moment one hairline grows. The rest of the line than contains two more integers: $p_i$ and $d_i$ ($1 \le p_i \le n$, $1 \le d_i \le 10^9$)&nbsp;— the number of the hairline and the length it grows by.</p>

## Output

<p>For each query of type $0$ print the time the haircut would take.</p>





```input1
4 7 3
1 2 3 4
0
1 2 3
0
1 1 3
0
1 3 1
0

```




```output1
1
2
2
1

```



## Note

<p>Consider the first example:</p><ul> <li> Initially lengths of hairlines are equal to $1, 2, 3, 4$ and only $4$-th hairline is longer $l=3$, and hairdresser can cut it in $1$ second. </li><li> Then Alice's second hairline grows, the lengths of hairlines are now equal to $1, 5, 3, 4$ </li><li> Now haircut takes two seonds: two swings are required: for the $4$-th hairline and for the $2$-nd. </li><li> Then Alice's first hairline grows, the lengths of hairlines are now equal to $4, 5, 3, 4$ </li><li> The haircut still takes two seconds: with one swing hairdresser can cut $4$-th hairline and with one more swing cut the segment from $1$-st to $2$-nd hairline. </li><li> Then Alice's third hairline grows, the lengths of hairlines are now equal to $4, 5, 4, 4$ </li><li> Now haircut takes only one second: with one swing it is possible to cut the segment from $1$-st hairline to the $4$-th. </li></ul>
