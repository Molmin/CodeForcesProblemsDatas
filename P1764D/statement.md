## Description

<div><p>Doremy has $n+1$ pegs. There are $n$ red pegs arranged as vertices of a regular $n$-sided polygon, numbered from $1$ to $n$ in anti-clockwise order. There is also a blue peg of <span class="tex-font-style-bf">slightly smaller diameter</span> in the middle of the polygon. A rubber band is stretched around the red pegs.</p><p>Doremy is very bored today and has decided to play a game. Initially, she has an empty array $a$. While the rubber band does not touch the blue peg, she will:</p><ol> <li> choose $i$ ($1 \leq i \leq n$) such that the red peg $i$ has not been removed; </li><li> remove the red peg $i$; </li><li> append $i$ to the back of $a$. </li></ol><p>Doremy wonders how many possible different arrays $a$ can be produced by the following process. Since the answer can be big, you are only required to output it modulo $p$. $p$ is guaranteed to be a prime number.</p><center>  <img class="tex-graphics" src="file://OnxD9scP.png" style="max-width: 100.0%;max-height: 100.0%;" width="360px">   <span class="tex-font-size-small">game with $n=9$ and $a=[7,5,2,8,3,9,4]$ and another game with $n=8$ and $a=[3,4,7,1,8,5,2]$</span> </center></div><div class="input-specification"><p>The first line contains two integers $n$ and $p$ ($3 \leq n \leq 5000$, $10^8 \le p \le 10^9$)&nbsp;— the number of red pegs and the modulo respectively.</p><p>$p$ is guaranteed to be a prime number.</p></div><div class="output-specification"><p>Output a single integer, the number of different arrays $a$ that can be produced by the process described above modulo $p$.</p></div>

## Input

<p>The first line contains two integers $n$ and $p$ ($3 \leq n \leq 5000$, $10^8 \le p \le 10^9$)&nbsp;— the number of red pegs and the modulo respectively.</p><p>$p$ is guaranteed to be a prime number.</p>

## Output

<p>Output a single integer, the number of different arrays $a$ that can be produced by the process described above modulo $p$.</p>





```input1
4 100000007
```




```input2
1145 141919831
```




```output1
16
```




```output2
105242108
```



## Note

<p>In the first test case, $n=4$, some possible arrays $a$ that can be produced are $[4,2,3]$ and $[1,4]$. However, it is not possible for $a$ to be $[1]$ or $[1,4,3]$.</p>
