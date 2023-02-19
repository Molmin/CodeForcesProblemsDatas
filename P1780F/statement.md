## Description

<div><p>One day Kira found $n$ friends from Morioh and decided to gather them around a table to have a peaceful conversation. The height of friend $i$ is equal to $a_i$. It so happened that the height of each of the friends <span class="tex-font-style-bf">is unique</span>.</p><p>Unfortunately, there were only $3$ chairs in Kira's house, and obviously, it will not be possible to seat all friends! So, Kira has to invite only $3$ of his friends.</p><p>But everything is not so simple! If the heights of the lowest and the tallest of the invited friends are not coprime, then the friends will play tricks on each other, which will greatly anger Kira.</p><p>Kira became interested, how many ways are there to choose $3$ of his friends so that they don't play tricks? Two ways are considered different if there is a friend invited in one way, but not in the other.</p><p>Formally, if Kira invites friends $i$, $j$, and $k$, then the following should be true: $\gcd(\min(a_i, a_j, a_k), \max(a_i, a_j, a_k)) = 1$, where $\gcd(x, y)$ denotes the <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor (GCD)</a> of the numbers $x$ and $y$.</p><p>Kira is not very strong in computer science, so he asks you to count the number of ways to invide friends.</p></div><div class="input-specification"><p>The first line contains the number $n$ ($3 \le n \le 3\cdot10^5$) — the number of Kira's friends.</p><p>The next line contains $n$ <span class="tex-font-style-bf">distinct</span> integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 3\cdot10^5$) — heights of Kira's friends.</p></div><div class="output-specification"><p>In a single line output the number of ways to invite three friends.</p></div>

## Input

<p>The first line contains the number $n$ ($3 \le n \le 3\cdot10^5$) — the number of Kira's friends.</p><p>The next line contains $n$ <span class="tex-font-style-bf">distinct</span> integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 3\cdot10^5$) — heights of Kira's friends.</p>

## Output

<p>In a single line output the number of ways to invite three friends.</p>





```input1
3
1 2 3
```




```input2
4
1 6 2 3
```




```input3
4
16 4 8 2
```




```input4
10
10 1 6 7 9 8 4 3 5 2
```




```output1
1
```




```output2
3
```




```output3
0
```




```output4
77
```



## Note

<p>In the first example, only one way is suitable: invite friends $1$, $2$, and $3$. Here $1 &lt; 2 &lt; 3$, and the numbers $1$ and $3$ are coprime.</p>
