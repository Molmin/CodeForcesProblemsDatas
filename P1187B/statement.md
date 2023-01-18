## Description

<div><p>The letters shop showcase is a string $s$, consisting of $n$ lowercase Latin letters. As the name tells, letters are sold in the shop.</p><p>Letters are sold one by one from the leftmost to the rightmost. Any customer can only buy some prefix of letters from the string $s$.</p><p>There are $m$ friends, the $i$-th of them is named $t_i$. Each of them is planning to estimate the following value: how many letters (the length of the shortest prefix) would s/he need to buy if s/he wanted to construct her/his name of bought letters. The name can be constructed if each letter is presented in the equal or greater amount.</p><ul> <li> For example, for $s$="<span class="tex-font-style-tt">arrayhead</span>" and $t_i$="<span class="tex-font-style-tt">arya</span>" $5$ letters have to be bought ("<span class="tex-font-style-tt"><span class="tex-font-style-bf">array</span>head</span>"). </li><li> For example, for $s$="<span class="tex-font-style-tt">arrayhead</span>" and $t_i$="<span class="tex-font-style-tt">harry</span>" $6$ letters have to be bought ("<span class="tex-font-style-tt"><span class="tex-font-style-bf">arrayh</span>ead</span>"). </li><li> For example, for $s$="<span class="tex-font-style-tt">arrayhead</span>" and $t_i$="<span class="tex-font-style-tt">ray</span>" $5$ letters have to be bought ("<span class="tex-font-style-tt"><span class="tex-font-style-bf">array</span>head</span>"). </li><li> For example, for $s$="<span class="tex-font-style-tt">arrayhead</span>" and $t_i$="<span class="tex-font-style-tt">r</span>" $2$ letters have to be bought ("<span class="tex-font-style-tt"><span class="tex-font-style-bf">ar</span>rayhead</span>"). </li><li> For example, for $s$="<span class="tex-font-style-tt">arrayhead</span>" and $t_i$="<span class="tex-font-style-tt">areahydra</span>" all $9$ letters have to be bought ("<span class="tex-font-style-tt"><span class="tex-font-style-bf">arrayhead</span></span>"). </li></ul><p>It is guaranteed that every friend can construct her/his name using the letters from the string $s$.</p><p>Note that the values for friends are independent, friends are only estimating them but not actually buying the letters.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the length of showcase string $s$.</p><p>The second line contains string $s$, consisting of exactly $n$ lowercase Latin letters.</p><p>The third line contains one integer $m$ ($1 \le m \le 5 \cdot 10^4$) — the number of friends.</p><p>The $i$-th of the next $m$ lines contains $t_i$ ($1 \le |t_i| \le 2 \cdot 10^5$) — the name of the $i$-th friend.</p><p>It is guaranteed that $\sum \limits_{i=1}^m |t_i| \le 2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each friend print the length of the shortest prefix of letters from $s$ s/he would need to buy to be able to construct her/his name of them. The name can be constructed if each letter is presented in the equal or greater amount.</p><p>It is guaranteed that every friend can construct her/his name using the letters from the string $s$.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the length of showcase string $s$.</p><p>The second line contains string $s$, consisting of exactly $n$ lowercase Latin letters.</p><p>The third line contains one integer $m$ ($1 \le m \le 5 \cdot 10^4$) — the number of friends.</p><p>The $i$-th of the next $m$ lines contains $t_i$ ($1 \le |t_i| \le 2 \cdot 10^5$) — the name of the $i$-th friend.</p><p>It is guaranteed that $\sum \limits_{i=1}^m |t_i| \le 2 \cdot 10^5$.</p>

## Output

<p>For each friend print the length of the shortest prefix of letters from $s$ s/he would need to buy to be able to construct her/his name of them. The name can be constructed if each letter is presented in the equal or greater amount.</p><p>It is guaranteed that every friend can construct her/his name using the letters from the string $s$.</p>





```input1
9
arrayhead
5
arya
harry
ray
r
areahydra
```




```output1
5
6
5
2
9
```


