## Description

<div><p>Medicine faculty of Berland State University has just finished their admission campaign. As usual, about $80\%$ of applicants are girls and majority of them are going to live in the university dormitory for the next $4$ (hopefully) years.</p><p>The dormitory consists of $n$ rooms and a single mouse! Girls decided to set mouse traps in some rooms to get rid of the horrible monster. Setting a trap in room number $i$ costs $c_i$ burles. Rooms are numbered from $1$ to $n$.</p><p>Mouse doesn't sit in place all the time, it constantly runs. If it is in room $i$ in second $t$ then it will run to room $a_i$ in second $t + 1$ without visiting any other rooms inbetween ($i = a_i$ means that mouse won't leave room $i$). It's second $0$ in the start. If the mouse is in some room with a mouse trap in it, then the mouse get caught into this trap.</p><p>That would have been so easy if the girls actually knew where the mouse at. Unfortunately, that's not the case, mouse can be in any room from $1$ to $n$ at second $0$.</p><p>What it the minimal total amount of burles girls can spend to set the traps in order to guarantee that the mouse will eventually be caught no matter the room it started from?</p></div><div class="input-specification"><p>The first line contains as single integers $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of rooms in the dormitory.</p><p>The second line contains $n$ integers $c_1, c_2, \dots, c_n$ ($1 \le c_i \le 10^4$) — $c_i$ is the cost of setting the trap in room number $i$.</p><p>The third line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$) — $a_i$ is the room the mouse will run to the next second after being in room $i$.</p></div><div class="output-specification"><p>Print a single integer — the minimal total amount of burles girls can spend to set the traps in order to guarantee that the mouse will eventually be caught no matter the room it started from.</p></div>

## Input

<p>The first line contains as single integers $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of rooms in the dormitory.</p><p>The second line contains $n$ integers $c_1, c_2, \dots, c_n$ ($1 \le c_i \le 10^4$) — $c_i$ is the cost of setting the trap in room number $i$.</p><p>The third line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$) — $a_i$ is the room the mouse will run to the next second after being in room $i$.</p>

## Output

<p>Print a single integer — the minimal total amount of burles girls can spend to set the traps in order to guarantee that the mouse will eventually be caught no matter the room it started from.</p>





```input1
5
1 2 3 2 10
1 3 4 3 3

```




```input2
4
1 10 2 10
2 4 2 2

```




```input3
7
1 1 1 1 1 1 1
2 2 2 3 6 7 6

```




```output1
3

```




```output2
10

```




```output3
2

```



## Note

<p>In the first example it is enough to set mouse trap in rooms $1$ and $4$. If mouse starts in room $1$ then it gets caught immideately. If mouse starts in any other room then it eventually comes to room $4$.</p><p>In the second example it is enough to set mouse trap in room $2$. If mouse starts in room $2$ then it gets caught immideately. If mouse starts in any other room then it runs to room $2$ in second $1$.</p><p>Here are the paths of the mouse from different starts from the third example:</p><ul> <li> $1 \rightarrow 2 \rightarrow 2 \rightarrow \dots$; </li><li> $2 \rightarrow 2 \rightarrow \dots$; </li><li> $3 \rightarrow 2 \rightarrow 2 \rightarrow \dots$; </li><li> $4 \rightarrow 3 \rightarrow 2 \rightarrow 2 \rightarrow \dots$; </li><li> $5 \rightarrow 6 \rightarrow 7 \rightarrow 6 \rightarrow \dots$; </li><li> $6 \rightarrow 7 \rightarrow 6 \rightarrow \dots$; </li><li> $7 \rightarrow 6 \rightarrow 7 \rightarrow \dots$; </li></ul><p>So it's enough to set traps in rooms $2$ and $6$.</p>
