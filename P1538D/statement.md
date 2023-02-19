## Description

<div><p>You are given two integers $a$ and $b$. In one turn, you can do one of the following operations: </p><ul> <li> Take an integer $c$ ($c &gt; 1$ and <span class="tex-font-style-bf">$a$ should be divisible by $c$</span>) and replace $a$ with $\frac{a}{c}$; </li><li> Take an integer $c$ ($c &gt; 1$ and <span class="tex-font-style-bf">$b$ should be divisible by $c$</span>) and replace $b$ with $\frac{b}{c}$. </li></ul><p>Your goal is to make $a$ equal to $b$ using exactly $k$ turns.</p><p>For example, the numbers $a=36$ and $b=48$ can be made equal in $4$ moves: </p><ul> <li> $c=6$, divide $b$ by $c$ $\Rightarrow$ $a=36$, $b=8$; </li><li> $c=2$, divide $a$ by $c$ $\Rightarrow$ $a=18$, $b=8$; </li><li> $c=9$, divide $a$ by $c$ $\Rightarrow$ $a=2$, $b=8$; </li><li> $c=4$, divide $b$ by $c$ $\Rightarrow$ $a=2$, $b=2$. </li></ul><p>For the given numbers $a$ and $b$, determine whether it is possible to make them equal using exactly $k$ turns.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^4$). Then $t$ test cases follow.</p><p>Each test case is contains three integers $a$, $b$ and $k$ ($1 \le a, b, k \le 10^9$).</p></div><div class="output-specification"><p>For each test case output: </p><ul> <li> "<span class="tex-font-style-tt">Yes</span>", if it is possible to make the numbers $a$ and $b$ equal in <span class="tex-font-style-bf">exactly</span> $k$ turns; </li><li> "<span class="tex-font-style-tt">No</span>" otherwise. </li></ul><p>The strings "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">No</span>" can be output in any case.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^4$). Then $t$ test cases follow.</p><p>Each test case is contains three integers $a$, $b$ and $k$ ($1 \le a, b, k \le 10^9$).</p>

## Output

<p>For each test case output: </p><ul> <li> "<span class="tex-font-style-tt">Yes</span>", if it is possible to make the numbers $a$ and $b$ equal in <span class="tex-font-style-bf">exactly</span> $k$ turns; </li><li> "<span class="tex-font-style-tt">No</span>" otherwise. </li></ul><p>The strings "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">No</span>" can be output in any case.</p>





```input1
8
36 48 2
36 48 3
36 48 4
2 8 1
2 8 2
1000000000 1000000000 1000000000
1 2 1
2 2 1
```




```output1
YES
YES
YES
YES
YES
NO
YES
NO
```


