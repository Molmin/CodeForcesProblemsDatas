## Description

<div><p>Little W and Little P decided to send letters to each other regarding the most important events during a day. There are $n$ events during a day: at time moment $t_i$ something happens to the person $p_i$ ($p_i$ is either <span class="tex-font-style-tt">W</span> or <span class="tex-font-style-tt">P</span>, denoting Little W and Little P, respectively), so he needs to immediately send a letter to the other person. They can send a letter using one of the two ways:</p><ul> <li> Ask Friendly O to deliver the letter directly. Friendly O takes $d$ acorns for each letter.</li><li> Leave the letter at Wise R's den. Wise R values free space, so he takes $c \cdot T$ acorns for storing a letter for a time segment of length $T$. The recipient can take a letter from Wise R either when he leaves his own letter at Wise R's den, or at time moment $t_{n + 1}$, when everybody comes to Wise R for a tea. It is not possible to take a letter from Wise R's den at other time moments. The friends can store as many letters at Wise R's den as they want, paying for each one separately. </li></ul><p>Help the friends determine the minimum possible total cost of sending all letters.</p></div><div class="input-specification"><p>The first line contains three integers $n, c, d$ ($1 \leq n \leq 10^5$, $1 \leq c \leq 10^2$, $1 \leq d \leq 10^8$)&nbsp;— the number of letters, the cost of storing a letter for one time unit at Wise R's den and the cost of delivering a letter via Friendly O.</p><p>The next $n$ describe the events. The $i$-th of them contains an integer $t_i$ and a character $p_i$ ($0 \leq t_i \leq 10^6$, $p_i$ is either <span class="tex-font-style-tt">W</span> or <span class="tex-font-style-tt">P</span>)&nbsp;— the time the $i$-th event happens and the person the event happens to.</p><p>The last line contains a single integer $t_{n + 1}$ ($0 \leq t_{n+1} \leq 10^6$)&nbsp;— the time when everybody comes to Wise R for a tea and takes all remaining letters. </p><p>It is guaranteed that $t_i &lt; t_{i + 1}$ for all $i$ from $1$ to $n$.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the minimum possible cost of delivery of all letters.</p></div>

## Input

<p>The first line contains three integers $n, c, d$ ($1 \leq n \leq 10^5$, $1 \leq c \leq 10^2$, $1 \leq d \leq 10^8$)&nbsp;— the number of letters, the cost of storing a letter for one time unit at Wise R's den and the cost of delivering a letter via Friendly O.</p><p>The next $n$ describe the events. The $i$-th of them contains an integer $t_i$ and a character $p_i$ ($0 \leq t_i \leq 10^6$, $p_i$ is either <span class="tex-font-style-tt">W</span> or <span class="tex-font-style-tt">P</span>)&nbsp;— the time the $i$-th event happens and the person the event happens to.</p><p>The last line contains a single integer $t_{n + 1}$ ($0 \leq t_{n+1} \leq 10^6$)&nbsp;— the time when everybody comes to Wise R for a tea and takes all remaining letters. </p><p>It is guaranteed that $t_i &lt; t_{i + 1}$ for all $i$ from $1$ to $n$.</p>

## Output

<p>Print a single integer&nbsp;— the minimum possible cost of delivery of all letters.</p>





```input1
5 1 4
0 P
1 W
3 P
5 P
8 P
10
```




```input2
10 10 94
17 W
20 W
28 W
48 W
51 P
52 W
56 W
62 P
75 P
78 P
87
```




```output1
16
```




```output2
916
```



## Note

<p>One of optimal solutions in the first example:</p><ul><li> At time moment 0 Little P leaves the letter at Wise R's den.</li><li> At time moment 1 Little W leaves his letter at Wise R's den and takes Little P's letter. This letter is at the den from time moment 0 to time moment 1, it costs $1$ acorn.</li><li> At time moment 3 Little P sends his letter via Friendly O, it costs $4$ acorns.</li><li> At time moment 5 Little P leaves his letter at the den, receiving Little W's letter which storage costs 4 acorns.</li><li> At time moment 8 Little P leaves one more letter at the den.</li><li> At time moment 10 Little W comes to the den for a tea and receives the two letters, paying 5 and 2 acorns.</li></ul><p>The total cost of delivery is thus $1 + 4 + 4 + 5 + 2 = 16$ acorns.</p>
