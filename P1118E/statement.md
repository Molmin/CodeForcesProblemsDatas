## Description

<div><p>The king of Berland organizes a ball! $n$ pair are invited to the ball, they are numbered from $1$ to $n$. Each pair consists of one man and one woman. Each dancer (either man or woman) has a monochrome costume. The color of each costume is represented by an integer from $1$ to $k$, inclusive.</p><p>Let $b_i$ be the color of the man's costume and $g_i$ be the color of the woman's costume in the $i$-th pair. You have to choose a color for each dancer's costume (i.e. values $b_1, b_2, \dots, b_n$ and $g_1, g_2, \dots g_n$) in such a way that:</p><ol> <li> for every $i$: $b_i$ and $g_i$ are integers between $1$ and $k$, inclusive; </li><li> there are no two completely identical pairs, i.e. no two indices $i, j$ ($i \ne j$) such that $b_i = b_j$ and $g_i = g_j$ at the same time; </li><li> there is no pair such that the color of the man's costume is the same as the color of the woman's costume in this pair, i.e. $b_i \ne g_i$ for every $i$; </li><li> for each two consecutive (adjacent) pairs both man's costume colors and woman's costume colors differ, i.e. for every $i$ from $1$ to $n-1$ the conditions $b_i \ne b_{i + 1}$ and $g_i \ne g_{i + 1}$ hold. </li></ol><p>Let's take a look at the examples of bad and good color choosing (for $n=4$ and $k=3$, man is the first in a pair and woman is the second):</p><p>Bad color choosing: </p><ul> <li> $(1, 2)$, $(2, 3)$, $(3, 2)$, $(1, 2)$ — contradiction with the second rule (there are equal pairs); </li><li> $(2, 3)$, $(1, 1)$, $(3, 2)$, $(1, 3)$ — contradiction with the third rule (there is a pair with costumes of the same color); </li><li> $(1, 2)$, $(2, 3)$, $(1, 3)$, $(2, 1)$ — contradiction with the fourth rule (there are two consecutive pairs such that colors of costumes of men/women are the same). </li></ul><p>Good color choosing: </p><ul> <li> $(1, 2)$, $(2, 1)$, $(1, 3)$, $(3, 1)$; </li><li> $(1, 2)$, $(3, 1)$, $(2, 3)$, $(3, 2)$; </li><li> $(3, 1)$, $(1, 2)$, $(2, 3)$, $(3, 2)$. </li></ul><p>You have to find <span class="tex-font-style-bf">any</span> suitable color choosing or say that no suitable choosing exists.</p></div><div class="input-specification"><p>The only line of the input contains two integers $n$ and $k$ ($2 \le n, k \le 2 \cdot 10^5$) — the number of pairs and the number of colors.</p></div><div class="output-specification"><p>If it is impossible to find <span class="tex-font-style-bf">any</span> suitable colors choosing, print "<span class="tex-font-style-tt">NO</span>".</p><p>Otherwise print "<span class="tex-font-style-tt">YES</span>" and then the colors of the costumes of pairs in the next $n$ lines. The $i$-th line should contain two integers $b_i$ and $g_i$ — colors of costumes of man and woman in the $i$-th pair, respectively.</p><p>You can print each letter in any case (upper or lower). For example, "<span class="tex-font-style-tt">YeS</span>", "<span class="tex-font-style-tt">no</span>" and "<span class="tex-font-style-tt">yES</span>" are all acceptable.</p></div>

## Input

<p>The only line of the input contains two integers $n$ and $k$ ($2 \le n, k \le 2 \cdot 10^5$) — the number of pairs and the number of colors.</p>

## Output

<p>If it is impossible to find <span class="tex-font-style-bf">any</span> suitable colors choosing, print "<span class="tex-font-style-tt">NO</span>".</p><p>Otherwise print "<span class="tex-font-style-tt">YES</span>" and then the colors of the costumes of pairs in the next $n$ lines. The $i$-th line should contain two integers $b_i$ and $g_i$ — colors of costumes of man and woman in the $i$-th pair, respectively.</p><p>You can print each letter in any case (upper or lower). For example, "<span class="tex-font-style-tt">YeS</span>", "<span class="tex-font-style-tt">no</span>" and "<span class="tex-font-style-tt">yES</span>" are all acceptable.</p>





```input1
4 3
```




```input2
10 4
```




```input3
13 4
```




```output1
YES
3 1
1 3
3 2
2 3
```




```output2
YES
2 1
1 3
4 2
3 4
4 3
3 2
2 4
4 1
1 4
3 1
```




```output3
NO
```


