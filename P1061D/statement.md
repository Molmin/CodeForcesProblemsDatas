## Description

<div><p>There are $n$ TV shows you want to watch. Suppose the whole time is split into equal parts called "minutes". The $i$-th of the shows is going from $l_i$-th to $r_i$-th minute, both ends inclusive.</p><p>You need a TV to watch a TV show and you can't watch two TV shows which air at the same time on the same TV, so it is possible you will need multiple TVs in some minutes. For example, if segments $[l_i, r_i]$ and $[l_j, r_j]$ intersect, then shows $i$ and $j$ can't be watched simultaneously on one TV.</p><p>Once you start watching a show on some TV it is not possible to "move" it to another TV (since it would be too distracting), or to watch another show on the same TV until this show ends.</p><p>There is a TV Rental shop near you. It rents a TV for $x$ rupees, and charges $y$ ($y &lt; x$) rupees for every extra minute you keep the TV. So in order to rent a TV for minutes $[a; b]$ you will need to pay $x + y \cdot (b - a)$. </p><p>You can assume, that taking and returning of the TV doesn't take any time and doesn't distract from watching other TV shows. Find the minimum possible cost to view all shows. Since this value could be too large, print it modulo $10^9 + 7$.</p></div><div class="input-specification"><p>The first line contains integers $n$, $x$ and $y$ ($1 \le n \le 10^5$, $1 \le y &lt; x \le 10^9$)&nbsp;— the number of TV shows, the cost to rent a TV for the first minute and the cost to rent a TV for every subsequent minute.</p><p>Each of the next $n$ lines contains two integers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le 10^9$) denoting the start and the end minute of the $i$-th TV show.</p></div><div class="output-specification"><p>Print exactly one integer&nbsp;— the minimum cost to view all the shows taken modulo $10^9 + 7$.</p></div>

## Input

<p>The first line contains integers $n$, $x$ and $y$ ($1 \le n \le 10^5$, $1 \le y &lt; x \le 10^9$)&nbsp;— the number of TV shows, the cost to rent a TV for the first minute and the cost to rent a TV for every subsequent minute.</p><p>Each of the next $n$ lines contains two integers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le 10^9$) denoting the start and the end minute of the $i$-th TV show.</p>

## Output

<p>Print exactly one integer&nbsp;— the minimum cost to view all the shows taken modulo $10^9 + 7$.</p>





```input1
5 4 3
1 2
4 10
2 4
10 11
5 9

```




```input2
6 3 2
8 20
6 22
4 15
20 28
17 25
20 27

```




```input3
2 1000000000 2
1 2
2 3

```




```output1
60
```




```output2
142
```




```output3
999999997
```



## Note

<p>In the first example, the optimal strategy would be to rent $3$ TVs to watch:</p><ul> <li> Show $[1, 2]$ on the first TV,</li><li> Show $[4, 10]$ on the second TV,</li><li> Shows $[2, 4], [5, 9], [10, 11]$ on the third TV. </li></ul><p>This way the cost for the first TV is $4 + 3 \cdot (2 - 1) = 7$, for the second is $4 + 3 \cdot (10 - 4) = 22$ and for the third is $4 + 3 \cdot (11 - 2) = 31$, which gives $60$ int total.</p><p>In the second example, it is optimal watch each show on a new TV.</p><p>In third example, it is optimal to watch both shows on a new TV. Note that the answer is to be printed modulo $10^9 + 7$.</p>
