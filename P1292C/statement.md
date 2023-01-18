## Description

<div><div class="epigraph"><div class="epigraph-text"><a href="https://www.youtube.com/watch?v=kwsciXm_7sA"><span class="tex-font-style-it">INSPION FullBand Master - INSPION</span></a></div></div> <div class="epigraph"><div class="epigraph-text"><a href="https://www.youtube.com/watch?v=kwsciXm_7sA"><span class="tex-font-style-it">INSPION - IOLITE-SUNSTONE</span></a></div></div><p>On another floor of the A.R.C. Markland-N, the young man Simon "Xenon" Jackson, takes a break after finishing his project early (as always). Having a lot of free time, he decides to put on his legendary hacker "X" instinct and fight against the gangs of the cyber world.</p><p>His target is a network of $n$ small gangs. This network contains exactly $n - 1$ direct links, each of them connecting two gangs together. The links are placed in such a way that every pair of gangs is connected through a sequence of direct links.</p><p>By mining data, Xenon figured out that the gangs used a form of cross-encryption to avoid being busted: every link was assigned an integer from $0$ to $n - 2$ such that all assigned integers are distinct and every integer was assigned to some link. If an intruder tries to access the encrypted data, they will have to surpass $S$ password layers, with $S$ being defined by the following formula:</p><p>$$S = \sum_{1 \leq u &lt; v \leq n} mex(u, v)$$</p><p>Here, $mex(u, v)$ denotes the smallest non-negative integer that does not appear on any link on the unique simple path from gang $u$ to gang $v$.</p><p>Xenon doesn't know the way the integers are assigned, but it's not a problem. He decides to let his AI's instances try all the passwords on his behalf, but before that, he needs to know the maximum possible value of $S$, so that the AIs can be deployed efficiently.</p><p>Now, Xenon is out to write the AI scripts, and he is expected to finish them in two hours. Can you find the maximum possible $S$ before he returns?</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($2 \leq n \leq 3000$), the number of gangs in the network.</p><p>Each of the next $n - 1$ lines contains integers $u_i$ and $v_i$ ($1 \leq u_i, v_i \leq n$; $u_i \neq v_i$), indicating there's a direct link between gangs $u_i$ and $v_i$.</p><p>It's guaranteed that links are placed in such a way that each pair of gangs will be connected by exactly one simple path.</p></div><div class="output-specification"><p>Print the maximum possible value of $S$&nbsp;— the number of password layers in the gangs' network.</p></div>

## Input

<p>The first line contains an integer $n$ ($2 \leq n \leq 3000$), the number of gangs in the network.</p><p>Each of the next $n - 1$ lines contains integers $u_i$ and $v_i$ ($1 \leq u_i, v_i \leq n$; $u_i \neq v_i$), indicating there's a direct link between gangs $u_i$ and $v_i$.</p><p>It's guaranteed that links are placed in such a way that each pair of gangs will be connected by exactly one simple path.</p>

## Output

<p>Print the maximum possible value of $S$&nbsp;— the number of password layers in the gangs' network.</p>





```input1
3
1 2
2 3
```




```input2
5
1 2
1 3
1 4
3 5
```




```output1
3
```




```output2
10
```



## Note

<p>In the first example, one can achieve the maximum $S$ with the following assignment:</p><center> <img class="tex-graphics" src="file://pRCsUFqA.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>With this assignment, $mex(1, 2) = 0$, $mex(1, 3) = 2$ and $mex(2, 3) = 1$. Therefore, $S = 0 + 2 + 1 = 3$.</p><p>In the second example, one can achieve the maximum $S$ with the following assignment:</p><center> <img class="tex-graphics" src="file://go8mbfH5.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>With this assignment, all non-zero mex value are listed below: </p><ul> <li> $mex(1, 3) = 1$ </li><li> $mex(1, 5) = 2$ </li><li> $mex(2, 3) = 1$ </li><li> $mex(2, 5) = 2$ </li><li> $mex(3, 4) = 1$ </li><li> $mex(4, 5) = 3$ </li></ul><p>Therefore, $S = 1 + 2 + 1 + 2 + 1 + 3 = 10$.</p>
