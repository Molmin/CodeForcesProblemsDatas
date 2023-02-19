## Description

<div><p>A lighthouse keeper Peter commands an army of $n$ battle lemmings. He ordered his army to stand in a line and numbered the lemmings from $1$ to $n$ from left to right. Some of the lemmings hold shields. Each lemming cannot hold more than one shield.</p><p>The more protected Peter's army is, the better. To calculate the <span class="tex-font-style-it">protection</span> of the army, he finds the number of protected pairs of lemmings, that is such pairs that both lemmings in the pair don't hold a shield, but there is a lemming with a shield between them.</p><p>Now it's time to prepare for defence and increase the protection of the army. To do this, Peter can give orders. He chooses a lemming with a shield and gives him one of the two orders: </p><ul> <li> give the shield to the left neighbor if it exists and doesn't have a shield; </li><li> give the shield to the right neighbor if it exists and doesn't have a shield. </li></ul><p>In one second Peter can give exactly one order.</p><p>It's not clear how much time Peter has before the defence. So he decided to determine the maximal value of army protection for each $k$ from $0$ to $\frac{n(n-1)}2$, if he gives no more that $k$ orders. Help Peter to calculate it!</p></div><div class="input-specification"><p>First line contains a single integer $n$ ($1 \le n \le 80$), the number of lemmings in Peter's army.</p><p>Second line contains $n$ integers $a_i$ ($0 \le a_i \le 1$). If $a_i = 1$, then the $i$-th lemming has a shield, otherwise $a_i = 0$.</p></div><div class="output-specification"><p>Print $\frac{n(n-1)}2 + 1$ numbers, the greatest possible protection after no more than $0, 1, \dots, \frac{n(n-1)}2$ orders.</p></div>

## Input

<p>First line contains a single integer $n$ ($1 \le n \le 80$), the number of lemmings in Peter's army.</p><p>Second line contains $n$ integers $a_i$ ($0 \le a_i \le 1$). If $a_i = 1$, then the $i$-th lemming has a shield, otherwise $a_i = 0$.</p>

## Output

<p>Print $\frac{n(n-1)}2 + 1$ numbers, the greatest possible protection after no more than $0, 1, \dots, \frac{n(n-1)}2$ orders.</p>





```input1
5
1 0 0 0 1
```




```input2
12
0 0 0 0 1 1 1 1 0 1 1 0
```




```output1
0 2 3 3 3 3 3 3 3 3 3
```




```output2
9 12 13 14 14 14 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15 15
```



## Note

<p>Consider the first example.</p><p>The protection is initially equal to zero, because for each pair of lemmings without shields there is no lemmings with shield.</p><p>In one second Peter can order the first lemming give his shield to the right neighbor. In this case, the protection is two, as there are two protected pairs of lemmings, $(1, 3)$ and $(1, 4)$.</p><p>In two seconds Peter can act in the following way. First, he orders the fifth lemming to give a shield to the left neighbor. Then, he orders the first lemming to give a shield to the right neighbor. In this case Peter has three protected pairs of lemmings&nbsp;— $(1, 3)$, $(1, 5)$ and $(3, 5)$.</p><p>You can make sure that it's impossible to give orders in such a way that the protection becomes greater than three.</p>
