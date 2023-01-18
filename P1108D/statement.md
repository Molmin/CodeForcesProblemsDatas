## Description

<div><p>You have a garland consisting of $n$ lamps. Each lamp is colored red, green or blue. The color of the $i$-th lamp is $s_i$ ('<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">G</span>' and '<span class="tex-font-style-tt">B</span>' — colors of lamps in the garland).</p><p>You have to recolor some lamps in this garland (recoloring a lamp means changing its initial color to another) in such a way that the obtained garland is <span class="tex-font-style-bf">diverse</span>.</p><p>A garland is called <span class="tex-font-style-bf">diverse</span> if any two adjacent (consecutive) lamps (i. e. such lamps that the distance between their positions is $1$) have distinct colors.</p><p>In other words, if the obtained garland is $t$ then for each $i$ from $1$ to $n-1$ the condition $t_i \ne t_{i + 1}$ should be satisfied.</p><p>Among all ways to recolor the initial garland to make it <span class="tex-font-style-bf">diverse</span> you have to choose one with the <span class="tex-font-style-bf">minimum</span> number of recolored lamps. If there are multiple optimal solutions, print <span class="tex-font-style-bf">any</span> of them.</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of lamps.</p><p>The second line of the input contains the string $s$ consisting of $n$ characters '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">G</span>' and '<span class="tex-font-style-tt">B</span>' — colors of lamps in the garland.</p></div><div class="output-specification"><p>In the first line of the output print one integer $r$ — the <span class="tex-font-style-bf">minimum</span> number of recolors needed to obtain a <span class="tex-font-style-bf">diverse</span> garland from the given one.</p><p>In the second line of the output print one string $t$ of length $n$ — a <span class="tex-font-style-bf">diverse</span> garland obtained from the initial one with <span class="tex-font-style-bf">minimum</span> number of recolors. If there are multiple optimal solutions, print <span class="tex-font-style-bf">any</span> of them.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of lamps.</p><p>The second line of the input contains the string $s$ consisting of $n$ characters '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">G</span>' and '<span class="tex-font-style-tt">B</span>' — colors of lamps in the garland.</p>

## Output

<p>In the first line of the output print one integer $r$ — the <span class="tex-font-style-bf">minimum</span> number of recolors needed to obtain a <span class="tex-font-style-bf">diverse</span> garland from the given one.</p><p>In the second line of the output print one string $t$ of length $n$ — a <span class="tex-font-style-bf">diverse</span> garland obtained from the initial one with <span class="tex-font-style-bf">minimum</span> number of recolors. If there are multiple optimal solutions, print <span class="tex-font-style-bf">any</span> of them.</p>





```input1
9
RBGRRBRGG
```




```input2
8
BBBGBRRR
```




```input3
13
BBRRRRGGGGGRR
```




```output1
2
RBGRGBRGR
```




```output2
2
BRBGBRGR
```




```output3
6
BGRBRBGBGBGRG
```


