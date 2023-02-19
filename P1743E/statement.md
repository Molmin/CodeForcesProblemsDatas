## Description

<div><p>Monocarp is playing a video game. In the game, he controls a spaceship and has to destroy an enemy spaceship.</p><p>Monocarp has two lasers installed on his spaceship. Both lasers $1$ and $2$ have two values: </p><ul> <li> $p_i$&nbsp;— the power of the laser; </li><li> $t_i$&nbsp;— the reload time of the laser. </li></ul><p>When a laser is fully charged, Monocarp can either shoot it or wait for the other laser to charge and shoot both of them at the same time.</p><p>An enemy spaceship has $h$ durability and $s$ shield capacity. When Monocarp shoots an enemy spaceship, it receives $(P - s)$ damage (i. e. $(P - s)$ gets subtracted from its durability), where $P$ is the total power of the lasers that Monocarp shoots (i. e. $p_i$ if he only shoots laser $i$ and $p_1 + p_2$ if he shoots both lasers at the same time). An enemy spaceship is considered destroyed when its durability becomes $0$ or lower.</p><p>Initially, both lasers are zero charged.</p><p>What's the lowest amount of time it can take Monocarp to destroy an enemy spaceship?</p></div><div class="input-specification"><p>The first line contains two integers $p_1$ and $t_1$ ($2 \le p_1 \le 5000$; $1 \le t_1 \le 10^{12}$)&nbsp;— the power and the reload time of the first laser.</p><p>The second line contains two integers $p_2$ and $t_2$ ($2 \le p_2 \le 5000$; $1 \le t_2 \le 10^{12}$)&nbsp;— the power and the reload time of the second laser.</p><p>The third line contains two integers $h$ and $s$ ($1 \le h \le 5000$; $1 \le s &lt; \min(p_1, p_2)$)&nbsp;— the durability and the shield capacity of an enemy spaceship. Note that the last constraint implies that Monocarp will always be able to destroy an enemy spaceship.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the lowest amount of time it can take Monocarp to destroy an enemy spaceship.</p></div>

## Input

<p>The first line contains two integers $p_1$ and $t_1$ ($2 \le p_1 \le 5000$; $1 \le t_1 \le 10^{12}$)&nbsp;— the power and the reload time of the first laser.</p><p>The second line contains two integers $p_2$ and $t_2$ ($2 \le p_2 \le 5000$; $1 \le t_2 \le 10^{12}$)&nbsp;— the power and the reload time of the second laser.</p><p>The third line contains two integers $h$ and $s$ ($1 \le h \le 5000$; $1 \le s &lt; \min(p_1, p_2)$)&nbsp;— the durability and the shield capacity of an enemy spaceship. Note that the last constraint implies that Monocarp will always be able to destroy an enemy spaceship.</p>

## Output

<p>Print a single integer&nbsp;— the lowest amount of time it can take Monocarp to destroy an enemy spaceship.</p>





```input1
5 10
4 9
16 1
```




```input2
10 1
5000 100000
25 9
```




```output1
20
```




```output2
25
```



## Note

<p>In the first example, Monocarp waits for both lasers to charge, then shoots both lasers at $10$, they deal $(5 + 4 - 1) = 8$ damage. Then he waits again and shoots lasers at $20$, dealing $8$ more damage.</p><p>In the second example, Monocarp doesn't wait for the second laser to charge. He just shoots the first laser $25$ times, dealing $(10 - 9) = 1$ damage each time.</p>
