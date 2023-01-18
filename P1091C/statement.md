## Description

<div><p>There are $n$ people sitting in a circle, numbered from $1$ to $n$ in the order in which they are seated. That is, for all $i$ from $1$ to $n-1$, the people with id $i$ and $i+1$ are adjacent. People with id $n$ and $1$ are adjacent as well.</p><p>The person with id $1$ initially has a ball. He picks a positive integer $k$ at most $n$, and passes the ball to his $k$-th neighbour in the direction of increasing ids, that person passes the ball to his $k$-th neighbour in the same direction, and so on until the person with the id $1$ gets the ball back. When he gets it back, people do not pass the ball any more.</p><p>For instance, if $n = 6$ and $k = 4$, the ball is passed in order $[1, 5, 3, 1]$. </p><p>Consider the set of all people that touched the ball. The <span class="tex-font-style-bf">fun value</span> of the game is the sum of the ids of people that touched it. In the above example, the <span class="tex-font-style-it">fun value</span> would be $1 + 5 + 3 = 9$.</p><p>Find and report the set of possible <span class="tex-font-style-it">fun values</span> for all choices of positive integer $k$. It can be shown that under the constraints of the problem, the ball always gets back to the $1$-st player after finitely many steps, and there are no more than $10^5$ possible <span class="tex-font-style-it">fun values</span> for given $n$.</p></div><div class="input-specification"><p>The only line consists of a single integer $n$&nbsp;($2 \leq n \leq 10^9$)&nbsp;— the number of people playing with the ball.</p></div><div class="output-specification"><p>Suppose the set of all <span class="tex-font-style-it">fun values</span> is $f_1, f_2, \dots, f_m$.</p><p>Output a single line containing $m$ space separated integers $f_1$ through $f_m$ in <span class="tex-font-style-bf">increasing</span> order.</p></div>

## Input

<p>The only line consists of a single integer $n$&nbsp;($2 \leq n \leq 10^9$)&nbsp;— the number of people playing with the ball.</p>

## Output

<p>Suppose the set of all <span class="tex-font-style-it">fun values</span> is $f_1, f_2, \dots, f_m$.</p><p>Output a single line containing $m$ space separated integers $f_1$ through $f_m$ in <span class="tex-font-style-bf">increasing</span> order.</p>





```input1
6
```




```input2
16
```




```output1
1 5 9 21
```




```output2
1 10 28 64 136
```



## Note

<p>In the first sample, we've already shown that picking $k = 4$ yields <span class="tex-font-style-it">fun value</span> $9$, as does $k = 2$. Picking $k = 6$ results in <span class="tex-font-style-it">fun value</span> of $1$. For $k = 3$ we get <span class="tex-font-style-it">fun value</span> $5$ and with $k = 1$ or $k = 5$ we get $21$. </p><center> <img class="tex-graphics" src="file://IiI7HYEP.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second sample, the values $1$, $10$, $28$, $64$ and $136$ are achieved for instance for $k = 16$, $8$, $4$, $10$ and $11$, respectively.</p>
