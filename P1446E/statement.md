## Description

<div><p>A patient has been infected with an unknown disease. His body can be seen as an infinite grid of triangular cells which looks as follows:</p><center> <img class="tex-graphics" src="file://mbvrYe1f.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Two cells are neighboring if they share a side. Therefore, each cell ($x$, $y$) has exactly three neighbors: </p><ul> <li> ($x+1$, $y$) </li><li> ($x-1$, $y$) </li><li> ($x+1$, $y-1$) if $x$ is even and ($x-1$, $y+1$) otherwise. </li></ul> <p>Initially some cells are infected, all the others are healthy. The process of recovery begins. Each second, for <span class="tex-font-style-bf">exactly one</span> cell (even though there might be multiple cells that could change its state) one of the following happens:</p><ul> <li> A healthy cell with at least $2$ infected neighbors also becomes infected. </li><li> An infected cell with at least $2$ healthy neighbors also becomes healthy. </li></ul><p>If no such cell exists, the process of recovery stops. Patient is considered recovered if the process of recovery has stopped and all the cells are healthy.</p><p>We're interested in a <span class="tex-font-style-bf">worst-case</span> scenario: is it possible that the patient never recovers, or if it's not possible, what is the maximum possible duration of the recovery process?</p></div><div class="input-specification"><p>The first line contains one integer $n$ $(1 \leq n \leq 250000)$ &nbsp;— the number of infected cells. </p><p>The $i$-th of the next $n$ lines contains two space-separated integers $x_i$ and $y_i$ $(0 \leq x_i, y_i &lt; 500)$, meaning that cell $(x_i, y_i)$ is infected. All cells $(x_i, y_i)$ are distinct, and all other cells are considered healthy. </p></div><div class="output-specification"><p>If it is possible that the organism never fully recovers from the disease, print <span class="tex-font-style-tt">SICK</span>. Otherwise, you should print <span class="tex-font-style-tt">RECOVERED</span> and in the next line an integer $k$ &nbsp;— the longest possible recovery period, modulo $998244353$. </p></div>

## Input

<p>The first line contains one integer $n$ $(1 \leq n \leq 250000)$ &nbsp;— the number of infected cells. </p><p>The $i$-th of the next $n$ lines contains two space-separated integers $x_i$ and $y_i$ $(0 \leq x_i, y_i &lt; 500)$, meaning that cell $(x_i, y_i)$ is infected. All cells $(x_i, y_i)$ are distinct, and all other cells are considered healthy. </p>

## Output

<p>If it is possible that the organism never fully recovers from the disease, print <span class="tex-font-style-tt">SICK</span>. Otherwise, you should print <span class="tex-font-style-tt">RECOVERED</span> and in the next line an integer $k$ &nbsp;— the longest possible recovery period, modulo $998244353$. </p>





```input1
4
0 0
1 0
2 0
0 1
```




```input2
3
1 0
3 0
1 1
```




```output1
RECOVERED
4
```




```output2
SICK
```



## Note

<p>For the first testcase, the following drawings describe the longest possible recovery process. It can be proven that there are no recovery periods of length $5$ or longer, and the organism always recovers in this testcase.</p><p><img class="tex-graphics" src="file://7AAQpNaH.png" style="max-width: 100.0%;max-height: 100.0%;"> $\hspace{40pt} \downarrow$ <img class="tex-graphics" src="file://5cPKpKvI.png" style="max-width: 100.0%;max-height: 100.0%;"> $\hspace{40pt} \downarrow$ <img class="tex-graphics" src="file://nB1c6Jcg.png" style="max-width: 100.0%;max-height: 100.0%;"> $\hspace{40pt} \downarrow$ <img class="tex-graphics" src="file://MYolVs7B.png" style="max-width: 100.0%;max-height: 100.0%;"> $\hspace{40pt} \downarrow$</p><p>$\hspace{15pt}$ RECOVERED</p><p>For the second testcase, it is possible for the cells $(2, 0)$, $(2, 1)$, $(0, 1)$ to become infected. After that, no cell can change its state, so the answer is <span class="tex-font-style-tt">SICK</span>, as not all of the cells are healthy.</p>
