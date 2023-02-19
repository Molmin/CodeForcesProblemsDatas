## Description

<div><p>Polycarp is editing a complicated computer program. First, variable $x$ is declared and assigned to $0$. Then there are instructions of two types: </p><ol> <li> <span class="tex-font-style-tt">set $y$ $v$</span>&nbsp;— assign $x$ a value $y$ or spend $v$ burles to remove that instruction (thus, not reassign $x$); </li><li> <span class="tex-font-style-tt">if $y$ $\dots$ end</span> block&nbsp;— execute instructions inside the <span class="tex-font-style-tt">if</span> block if the value of $x$ is $y$ and ignore the block otherwise. </li></ol><p><span class="tex-font-style-tt">if</span> blocks can contain <span class="tex-font-style-tt">set</span> instructions and other <span class="tex-font-style-tt">if</span> blocks inside them.</p><p>However, when the value of $x$ gets assigned to $s$, the computer breaks and immediately catches fire. Polycarp wants to prevent that from happening and spend as few burles as possible.</p><p>What is the minimum amount of burles he can spend on removing <span class="tex-font-style-tt">set</span> instructions to never assign $x$ to $s$?</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $s$ ($1 \le n \le 2 \cdot 10^5$, $1 \le s \le 2 \cdot 10^5$)&nbsp;— the number of lines in the program and the forbidden value of $x$.</p><p>The following $n$ lines describe the program. Each line is one of three types: </p><ol> <li> <span class="tex-font-style-tt">set $y$ $v$</span> $(0 \le y \le 2 \cdot 10^5, 1 \le v \le 10^9)$; </li><li> <span class="tex-font-style-tt">if $y$</span> $(0 \le y \le 2 \cdot 10^5)$; </li><li> <span class="tex-font-style-tt">end</span>. </li></ol><p>Each <span class="tex-font-style-tt">if</span> instruction is matched by an <span class="tex-font-style-tt">end</span> instruction. Each <span class="tex-font-style-tt">end</span> instruction has an <span class="tex-font-style-tt">if</span> instruction to match.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the minimum amount of burles Polycarp can spend on removing <span class="tex-font-style-tt">set</span> instructions to never assign $x$ to $s$.</p></div>

## Input

<p>The first line contains two integers $n$ and $s$ ($1 \le n \le 2 \cdot 10^5$, $1 \le s \le 2 \cdot 10^5$)&nbsp;— the number of lines in the program and the forbidden value of $x$.</p><p>The following $n$ lines describe the program. Each line is one of three types: </p><ol> <li> <span class="tex-font-style-tt">set $y$ $v$</span> $(0 \le y \le 2 \cdot 10^5, 1 \le v \le 10^9)$; </li><li> <span class="tex-font-style-tt">if $y$</span> $(0 \le y \le 2 \cdot 10^5)$; </li><li> <span class="tex-font-style-tt">end</span>. </li></ol><p>Each <span class="tex-font-style-tt">if</span> instruction is matched by an <span class="tex-font-style-tt">end</span> instruction. Each <span class="tex-font-style-tt">end</span> instruction has an <span class="tex-font-style-tt">if</span> instruction to match.</p>

## Output

<p>Print a single integer&nbsp;— the minimum amount of burles Polycarp can spend on removing <span class="tex-font-style-tt">set</span> instructions to never assign $x$ to $s$.</p>





```input1
5 1
set 1 10
set 2 15
if 2
set 1 7
end
```




```input2
7 2
set 3 4
if 3
set 10 4
set 2 7
set 10 1
end
set 4 2
```




```input3
9 200
if 0
set 5 5
if 5
set 100 13
end
if 100
set 200 1
end
end
```




```input4
1 10
set 1 15
```




```output1
17
```




```output2
4
```




```output3
1
```




```output4
0
```


