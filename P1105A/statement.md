## Description

<div><p>Salem gave you $n$ sticks with integer positive lengths $a_1, a_2, \ldots, a_n$.</p><p>For every stick, you can change its length to any other positive integer length (that is, either shrink or stretch it). The cost of changing the stick's length from $a$ to $b$ is $|a - b|$, where $|x|$ means the absolute value of $x$.</p><p>A stick length $a_i$ is called <span class="tex-font-style-it">almost good</span> for some integer $t$ if $|a_i - t| \le 1$.</p><p>Salem asks you to change the lengths of some sticks (possibly all or none), such that all sticks' lengths are almost good for some positive integer $t$ and the total cost of changing is minimum possible. The value of $t$ is not fixed in advance and you can choose it as any positive integer. </p><p>As an answer, print the value of $t$ and the minimum cost. If there are multiple optimal choices for $t$, print any of them.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 1000$)&nbsp;— the number of sticks.</p><p>The second line contains $n$ integers $a_i$ ($1 \le a_i \le 100$)&nbsp;— the lengths of the sticks.</p></div><div class="output-specification"><p>Print the value of $t$ and the minimum possible cost. If there are multiple optimal choices for $t$, print any of them.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 1000$)&nbsp;— the number of sticks.</p><p>The second line contains $n$ integers $a_i$ ($1 \le a_i \le 100$)&nbsp;— the lengths of the sticks.</p>

## Output

<p>Print the value of $t$ and the minimum possible cost. If there are multiple optimal choices for $t$, print any of them.</p>





```input1
3
10 1 4
```




```input2
5
1 1 2 2 3
```




```output1
3 7
```




```output2
2 0
```



## Note

<p>In the first example, we can change $1$ into $2$ and $10$ into $4$ with cost $|1 - 2| + |10 - 4| = 1 + 6 = 7$ and the resulting lengths $[2, 4, 4]$ are almost good for $t = 3$.</p><p>In the second example, the sticks lengths are already almost good for $t = 2$, so we don't have to do anything.</p>
