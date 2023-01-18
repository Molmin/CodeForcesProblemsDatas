## Description

<div><p>There are $n$ children, who study at the school №41. It is well-known that they are good mathematicians. Once at a break, they arranged a challenge for themselves. All children arranged in a row and turned heads either to the left or to the right.</p><p>Children can do the following: in one second&nbsp;several pairs of neighboring children who are <span class="tex-font-style-bf">looking at each other</span> can <span class="tex-font-style-bf">simultaneously</span> turn the head in the opposite direction. For instance, the one who was looking at the right neighbor turns left and vice versa for the second child. Moreover, every second <span class="tex-font-style-bf">at least one</span> pair of neighboring children performs such action. They are going to finish when there is no pair of neighboring children who are looking at each other. </p><p>You are given the number $n$, the initial arrangement of children and the number $k$. You have to find a way for the children to act if they want to finish the process in exactly $k$ seconds. More formally, for each of the $k$ moves, you need to output the numbers of the children who turn left during this move.</p><p>For instance, for the configuration shown below and $k = 2$ children can do the following steps: </p><center> <img class="tex-graphics" src="file://lWtnLEnK.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> At the beginning, two pairs make move: $(1, 2)$ and $(3, 4)$. After that, we receive the following configuration: <center> <img class="tex-graphics" src="file://W6r9id1t.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> At the second move pair $(2, 3)$ makes the move. The final configuration is reached. Good job. <center> <img class="tex-graphics" src="file://Y1hTNizv.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>It is guaranteed that if the solution exists, it takes not more than $n^2$ "headturns".</p></div><div class="input-specification"><p>The first line of input contains two integers $n$ and $k$ ($2 \le n \le 3000$, $1 \le k \le 3000000$) &nbsp;— the number of children and required number of moves.</p><p>The next line contains a string of length $n$ and consists only of characters <span class="tex-font-style-tt">L</span> and <span class="tex-font-style-tt">R</span>, where <span class="tex-font-style-tt">L</span> means that the child looks to the left and <span class="tex-font-style-tt">R</span> means that the child looks to the right. </p></div><div class="output-specification"><p>If there is no solution, print a single line with number $-1$.</p><p>Otherwise, output $k$ lines. Each line has to start with a number $n_i$ ($1\le n_i \le \frac{n}{2}$) &nbsp;— the number of pairs of children, who turn at this move. After that print $n_i$ <span class="tex-font-style-bf">distinct</span> integers &nbsp;— the numbers of the children who will turn left during this move. </p><p>After performing all "headturns", there can't be a pair of two neighboring children looking at each other.</p><p>If there are many solutions, print any of them.</p></div>

## Input

<p>The first line of input contains two integers $n$ and $k$ ($2 \le n \le 3000$, $1 \le k \le 3000000$) &nbsp;— the number of children and required number of moves.</p><p>The next line contains a string of length $n$ and consists only of characters <span class="tex-font-style-tt">L</span> and <span class="tex-font-style-tt">R</span>, where <span class="tex-font-style-tt">L</span> means that the child looks to the left and <span class="tex-font-style-tt">R</span> means that the child looks to the right. </p>

## Output

<p>If there is no solution, print a single line with number $-1$.</p><p>Otherwise, output $k$ lines. Each line has to start with a number $n_i$ ($1\le n_i \le \frac{n}{2}$) &nbsp;— the number of pairs of children, who turn at this move. After that print $n_i$ <span class="tex-font-style-bf">distinct</span> integers &nbsp;— the numbers of the children who will turn left during this move. </p><p>After performing all "headturns", there can't be a pair of two neighboring children looking at each other.</p><p>If there are many solutions, print any of them.</p>





```input1
2 1
RL
```




```input2
2 1
LR
```




```input3
4 2
RLRL
```




```output1
1 1
```




```output2
-1
```




```output3
2 1 3 
1 2
```



## Note

<p>The first sample contains a pair of children who look at each other. After one move, they can finish the process.</p><p>In the second sample, children can't make any move. As a result, they can't end in $k&gt;0$ moves.</p><p>The third configuration is described in the statement.</p>
