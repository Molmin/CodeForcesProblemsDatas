## Description

<div><p>The campus has $m$ rooms numbered from $0$ to $m - 1$. Also the $x$-mouse lives in the campus. The $x$-mouse is not just a mouse: each second $x$-mouse moves from room $i$ to the room $i \cdot x \mod{m}$ (in fact, it teleports from one room to another since it doesn't visit any intermediate room). Starting position of the $x$-mouse is unknown.</p><p>You are responsible to catch the $x$-mouse in the campus, so you are guessing about minimum possible number of traps (one trap in one room) you need to place. You are sure that if the $x$-mouse enters a trapped room, it immediately gets caught.</p><p>And the only observation you made is $\text{GCD} (x, m) = 1$.</p></div><div class="input-specification"><p>The only line contains two integers $m$ and $x$ ($2 \le m \le 10^{14}$, $1 \le x &lt; m$, $\text{GCD} (x, m) = 1$) — the number of rooms and the parameter of $x$-mouse. </p></div><div class="output-specification"><p>Print the only integer — minimum number of traps you need to install to catch the $x$-mouse.</p></div>

## Input

<p>The only line contains two integers $m$ and $x$ ($2 \le m \le 10^{14}$, $1 \le x &lt; m$, $\text{GCD} (x, m) = 1$) — the number of rooms and the parameter of $x$-mouse. </p>

## Output

<p>Print the only integer — minimum number of traps you need to install to catch the $x$-mouse.</p>





```input1
4 3

```




```input2
5 2

```




```output1
3

```




```output2
2

```



## Note

<p>In the first example you can, for example, put traps in rooms $0$, $2$, $3$. If the $x$-mouse starts in one of this rooms it will be caught immediately. If $x$-mouse starts in the $1$-st rooms then it will move to the room $3$, where it will be caught.</p><p>In the second example you can put one trap in room $0$ and one trap in any other room since $x$-mouse will visit all rooms $1..m-1$ if it will start in any of these rooms.</p>
