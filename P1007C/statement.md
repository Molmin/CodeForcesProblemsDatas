## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem.</span></p><p>Vasya and Vitya play a game. Vasya thought of two integers $a$ and $b$ from $1$ to $n$ and Vitya tries to guess them. Each round he tells Vasya two numbers $x$ and $y$ from $1$ to $n$. If both $x=a$ and $y=b$ then Vitya wins. Else Vasya must say one of the three phrases: </p><ol> <li> $x$ is less than $a$; </li><li> $y$ is less than $b$; </li><li> $x$ is greater than $a$ or $y$ is greater than $b$. </li></ol><p>Vasya can't lie, but if multiple phrases are true, he may choose any of them. For example, if Vasya thought of numbers $2$ and $4$, then he answers with the phrase $3$ to a query $(3, 4)$, and he can answer with the phrase $1$ or phrase $3$ to a query $(1, 5)$.</p><p>Help Vitya win in no more than $600$ rounds. </p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \leq n \leq 10^{18}$)&nbsp;— the upper limit of the numbers.</p></div><div><h2>Interaction</h2><p>First, you need to read the number $n$, after that you can make queries.</p><p>To make a query, print two integers: $x$ and $y$ ($1 \leq x, y \leq n$), then <span class="tex-font-style-tt">flush</span> the output.</p><p>After each query, read a single integer $ans$ ($0 \leq ans \leq 3$).</p><p>If $ans &gt; 0$, then it is the number of the phrase said by Vasya.</p><p>If $ans = 0$, it means that you win and your program should terminate.</p><p>If you make more than $600$ queries or make an incorrect query, you will get <span class="tex-font-style-tt">Wrong Answer</span>.</p><p>Your solution will get <span class="tex-font-style-tt">Idleness Limit Exceeded</span>, if you don't print anything or forget to <span class="tex-font-style-tt">flush</span> the output.</p><p>To <span class="tex-font-style-tt">flush</span> you need to do the following right after printing a query and a line end: </p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> For other languages see documentation. </li></ul><p><span class="tex-font-style-bf">Hacks format</span></p><p>For hacks, use the following format:</p><p>In the first line, print a single integer $n$ ($1 \leq n \leq 10^{18}$)&nbsp;— the upper limit of the numbers.</p><p>In the second line, print two integers $a$ and $b$ ($1 \leq a, b \leq n$)&nbsp;— the numbers which Vasya thought of.</p><p>In the third line, print a single integer $m$ ($1 \leq m \leq 10^5$)&nbsp;— the number of instructions for the interactor.</p><p>In each of the next $m$ lines, print five integers: $x_i$, $y_i$, $r^{12}_i$, $r^{13}_i$, and $r^{23}_i$ ($1 \leq x_i, y_i \leq n$), where $r^{ST}_i$ equals to either number $S$ or number $T$.</p><p>While answering the query $x\,\, y$, the interactor finds a number $i$ from $1$ to $n$ with the minimal value $|x-x_i| + |y-y_i|$. If multiple numbers can be chosen, the least $i$ is preferred. Then the interactor answers to the query, but if there are two phrases $S$ and $T$ that can be given, then $r^{ST}_i$ is chosen.</p><p>For example, the sample test data file contains the following: </p><pre class="verbatim"><br>5<br>2 4<br>2<br>2 5 1 1 2<br>4 1 2 3 3<br></pre></div>

## Input

<p>The first line contains a single integer $n$ ($1 \leq n \leq 10^{18}$)&nbsp;— the upper limit of the numbers.</p>





```input1
5
3
3
2
1
0
```




```output1
4 3
3 4
3 3
1 5
2 4
```



## Note

<p>Let's analyze the sample test. The chosen numbers are $2$ and $4$. The interactor was given two instructions.</p><p>For the query $(4, 3)$, it can return $2$ or $3$. Out of the two instructions the second one is chosen, so the interactor returns $a^{23}_2=3$.</p><p>For the query $(3, 4)$, it can return only $3$.</p><p>For the query $(3, 3)$, it can return $2$ or $3$. Out of the two instructions the first one is chosen (since in case of equal values, the least number is preferred), so the interactor returns $a^{23}_1=2$.</p><p>For the query $(1, 5)$, it can return $1$ or $3$. Out of the two instructions the first one is chosen, so the interactor returns $a^{13}_1=1$.</p><p>In the fifth query $(2, 4)$, the numbers are guessed correctly, the player wins.</p>
