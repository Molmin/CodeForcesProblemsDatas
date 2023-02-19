## Description

<div><p>Monocarp is playing a computer game. He's going to kill $n$ monsters, the $i$-th of them has $h_i$ health.</p><p>Monocarp's character has two spells, either of which he can cast an arbitrary number of times (possibly, zero) and in an arbitrary order: </p><ul> <li> choose exactly two alive monsters and decrease their health by $1$; </li><li> choose a single monster and kill it. </li></ul><p>When a monster's health becomes $0$, it dies.</p><p>What's the minimum number of spell casts Monocarp should perform in order to kill all monsters?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains a single integer $n$ ($1 \le n \le 100$)&nbsp;— the number of monsters.</p><p>The second line contains $n$ integers $h_1, h_2, \dots, h_n$ ($1 \le h_i \le 100$)&nbsp;— the health of each monster.</p><p>The sum of $n$ over all testcases doesn't exceed $2 \cdot 10^4$.</p></div><div class="output-specification"><p>For each testcase, print a single integer&nbsp;— the minimum number of spell casts Monocarp should perform in order to kill all monsters.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains a single integer $n$ ($1 \le n \le 100$)&nbsp;— the number of monsters.</p><p>The second line contains $n$ integers $h_1, h_2, \dots, h_n$ ($1 \le h_i \le 100$)&nbsp;— the health of each monster.</p><p>The sum of $n$ over all testcases doesn't exceed $2 \cdot 10^4$.</p>

## Output

<p>For each testcase, print a single integer&nbsp;— the minimum number of spell casts Monocarp should perform in order to kill all monsters.</p>





```input1|2,3,6,7
3
4
1 2 1 2
3
2 4 2
5
1 2 3 4 5
```




```output1
3
3
5
```



## Note

<p>In the first testcase, the initial health list is $[1, 2, 1, 2]$. Three spells are casted: </p><ul> <li> the first spell on monsters $1$ and $2$&nbsp;— monster $1$ dies, monster $2$ has now health $1$, new health list is $[0, 1, 1, 2]$; </li><li> the first spell on monsters $3$ and $4$&nbsp;— monster $3$ dies, monster $4$ has now health $1$, new health list is $[0, 1, 0, 1]$; </li><li> the first spell on monsters $2$ and $4$&nbsp;— both monsters $2$ and $4$ die. </li></ul><p>In the second testcase, the initial health list is $[2, 4, 2]$. Three spells are casted: </p><ul> <li> the first spell on monsters $1$ and $3$&nbsp;— both monsters have health $1$ now, new health list is $[1, 4, 1]$; </li><li> the second spell on monster $2$&nbsp;— monster $2$ dies, new health list is $[1, 0, 1]$; </li><li> the first spell on monsters $1$ and $3$&nbsp;— both monsters $1$ and $3$ die. </li></ul><p>In the third testcase, the initial health list is $[1, 2, 3, 4, 5]$. Five spells are casted. The $i$-th of them kills the $i$-th monster with the second spell. Health list sequence: $[1, 2, 3, 4, 5]$ $\rightarrow$ $[0, 2, 3, 4, 5]$ $\rightarrow$ $[0, 0, 3, 4, 5]$ $\rightarrow$ $[0, 0, 0, 4, 5]$ $\rightarrow$ $[0, 0, 0, 0, 5]$ $\rightarrow$ $[0, 0, 0, 0, 0]$.</p>
