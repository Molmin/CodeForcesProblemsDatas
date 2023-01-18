## Description

<div><p><span class="tex-font-style-it">The three friends, Kuro, Shiro, and Katie, met up again! It's time for a party...</span></p><p>What the cats do when they unite? Right, they have a party. Since they wanted to have as much fun as possible, they invited all their friends. Now $n$ cats are at the party, sitting in a circle and eating soup. The rules are simple: anyone having finished their soup leaves the circle.</p><p>Katie suddenly notices that whenever a cat leaves, the place where she was sitting becomes an empty space, which means the circle is divided into smaller continuous groups of cats sitting next to each other. At the moment Katie observes, there are $m$ cats who left the circle. This raises a question for Katie: what is the maximum possible number of groups the circle is divided into at the moment?</p><p>Could you help her with this curiosity?</p><p>You can see the examples and their descriptions with pictures in the "Note" section.</p></div><div class="input-specification"><p>The only line contains two integers $n$ and $m$ ($2 \leq n \leq 1000$, $0 \leq m \leq n$)&nbsp;— the initial number of cats at the party and the number of cats who left the circle at the moment Katie observes, respectively.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the maximum number of groups of cats at the moment Katie observes.</p></div>

## Input

<p>The only line contains two integers $n$ and $m$ ($2 \leq n \leq 1000$, $0 \leq m \leq n$)&nbsp;— the initial number of cats at the party and the number of cats who left the circle at the moment Katie observes, respectively.</p>

## Output

<p>Print a single integer&nbsp;— the maximum number of groups of cats at the moment Katie observes.</p>





```input1
7 4
```




```input2
6 2
```




```input3
3 0
```




```input4
2 2
```




```output1
3
```




```output2
2
```




```output3
1
```




```output4
0
```



## Note

<p>In the first example, originally there are $7$ cats sitting as shown below, creating a single group:</p><center> <img class="tex-graphics" src="file://6LceRmCM.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>At the observed moment, $4$ cats have left the table. Suppose the cats $2$, $3$, $5$ and $7$ have left, then there are $3$ groups remaining. It is possible to show that it is the maximum possible number of groups remaining.</p><center> <img class="tex-graphics" src="file://P8L2aOlT.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second example, there are $6$ cats sitting as shown below:</p><center> <img class="tex-graphics" src="file://REdpOJOa.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>At the observed moment, $2$ cats have left the table. Suppose the cats numbered $3$ and $6$ left, then there will be $2$ groups remaining ($\{1, 2\}$ and $\{4, 5\}$). It is impossible to have more than $2$ groups of cats remaining.</p><center> <img class="tex-graphics" src="file://6WxVMZFI.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the third example, no cats have left, so there is $1$ group consisting of all cats.</p><p>In the fourth example, all cats have left the circle, so there are $0$ groups.</p>
