## Description

<div><p>Andi and Budi were given an assignment to tidy up their bookshelf of $n$ books. Each book is represented by the book title — a string $s_i$ numbered from $1$ to $n$, each with length $m$. Andi really wants to sort the book lexicographically ascending, while Budi wants to sort it lexicographically descending.</p><p>Settling their fight, they decided to combine their idea and sort it <span class="tex-font-style-it">asc-desc-endingly</span>, where <span class="tex-font-style-bf">the odd-indexed characters will be compared ascendingly</span>, and <span class="tex-font-style-bf">the even-indexed characters will be compared descendingly</span>.</p><p>A string $a$ occurs before a string $b$ in <span class="tex-font-style-it">asc-desc-ending</span> order if and only if in the first position where $a$ and $b$ differ, the following holds:</p><ul> <li> if it is an odd position, the string $a$ has a letter that appears earlier in the alphabet than the corresponding letter in $b$; </li><li> if it is an even position, the string $a$ has a letter that appears later in the alphabet than the corresponding letter in $b$. </li></ul></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \leq n \cdot m \leq 10^6$).</p><p>The $i$-th of the next $n$ lines contains a string $s_i$ consisting of $m$ uppercase Latin letters — the book title. The strings are pairwise distinct.</p></div><div class="output-specification"><p>Output $n$ integers — the indices of the strings after they are sorted <span class="tex-font-style-it">asc-desc-endingly</span>.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \leq n \cdot m \leq 10^6$).</p><p>The $i$-th of the next $n$ lines contains a string $s_i$ consisting of $m$ uppercase Latin letters — the book title. The strings are pairwise distinct.</p>

## Output

<p>Output $n$ integers — the indices of the strings after they are sorted <span class="tex-font-style-it">asc-desc-endingly</span>.</p>





```input1
5 2
AA
AB
BB
BA
AZ
```




```output1
5 2 1 3 4
```



## Note

<p>The following illustrates the first example.</p><center> <img class="tex-graphics" src="file://5RiuSXol.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
