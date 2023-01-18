## Description

<div><p>You have a garland consisting of $n$ lamps. Each lamp is colored red, green or blue. The color of the $i$-th lamp is $s_i$ ('<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">G</span>' and '<span class="tex-font-style-tt">B</span>' — colors of lamps in the garland).</p><p>You have to recolor some lamps in this garland (recoloring a lamp means changing its initial color to another) in such a way that the obtained garland is <span class="tex-font-style-bf">nice</span>.</p><p>A garland is called <span class="tex-font-style-bf">nice</span> if any two lamps of the same color have distance divisible by three between them. I.e. if the obtained garland is $t$, then for each $i, j$ such that $t_i = t_j$ should be satisfied $|i-j|~ mod~ 3 = 0$. The value $|x|$ means absolute value of $x$, the operation $x~ mod~ y$ means remainder of $x$ when divided by $y$.</p><p>For example, the following garlands are <span class="tex-font-style-bf">nice</span>: "<span class="tex-font-style-tt">RGBRGBRG</span>", "<span class="tex-font-style-tt">GB</span>", "<span class="tex-font-style-tt">R</span>", "<span class="tex-font-style-tt">GRBGRBG</span>", "<span class="tex-font-style-tt">BRGBRGB</span>". The following garlands are not <span class="tex-font-style-bf">nice</span>: "<span class="tex-font-style-tt">RR</span>", "<span class="tex-font-style-tt">RGBG</span>".</p><p>Among all ways to recolor the initial garland to make it <span class="tex-font-style-bf">nice</span> you have to choose one with the <span class="tex-font-style-bf">minimum</span> number of recolored lamps. If there are multiple optimal solutions, print <span class="tex-font-style-bf">any</span> of them.</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of lamps.</p><p>The second line of the input contains the string $s$ consisting of $n$ characters '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">G</span>' and '<span class="tex-font-style-tt">B</span>' — colors of lamps in the garland.</p></div><div class="output-specification"><p>In the first line of the output print one integer $r$ — the <span class="tex-font-style-bf">minimum</span> number of recolors needed to obtain a <span class="tex-font-style-bf">nice</span> garland from the given one.</p><p>In the second line of the output print one string $t$ of length $n$ — a <span class="tex-font-style-bf">nice</span> garland obtained from the initial one with <span class="tex-font-style-bf">minimum</span> number of recolors. If there are multiple optimal solutions, print <span class="tex-font-style-bf">any</span> of them.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of lamps.</p><p>The second line of the input contains the string $s$ consisting of $n$ characters '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">G</span>' and '<span class="tex-font-style-tt">B</span>' — colors of lamps in the garland.</p>

## Output

<p>In the first line of the output print one integer $r$ — the <span class="tex-font-style-bf">minimum</span> number of recolors needed to obtain a <span class="tex-font-style-bf">nice</span> garland from the given one.</p><p>In the second line of the output print one string $t$ of length $n$ — a <span class="tex-font-style-bf">nice</span> garland obtained from the initial one with <span class="tex-font-style-bf">minimum</span> number of recolors. If there are multiple optimal solutions, print <span class="tex-font-style-bf">any</span> of them.</p>





```input1
3
BRB
```




```input2
7
RGBGRBB
```




```output1
1
GRB
```




```output2
3
RGBRGBR
```


