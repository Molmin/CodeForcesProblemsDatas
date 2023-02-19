## Description

<div><p>Vittorio has three favorite toys: a teddy bear, an owl, and a raccoon. Each of them has a name. </p><p>Vittorio takes several sheets of paper and writes a letter on each side of every sheet so that it is possible to spell any of the three names by arranging some of the sheets in a row (sheets can be reordered and flipped as needed). The three names do not have to be spelled at the same time, it is sufficient that it is possible to spell each of them using all the available sheets (and the same sheet can be used to spell different names).</p><p>Find the minimum number of sheets required. In addition, produce a list of sheets with minimum cardinality which can be used to spell the three names (if there are multiple answers, print any).</p></div><div class="input-specification"><p>The first line contains a string $t$ consisting of uppercase letters of the English alphabet ($1\le |t| \le 1000$) — the name of the teddy bear.</p><p>The second line contains a string $o$ consisting of uppercase letters of the English alphabet ($1\le |o| \le 1000$) — the name of the owl.</p><p>The third line contains a string $r$ consisting of uppercase letters of the English alphabet ($1\le |r| \le 1000$) — the name of the raccoon.</p><p>The values $|t|$, $|o|$, $|r|$ denote the length of the three names $t$, $o$, $r$.</p></div><div class="output-specification"><p>The first line of the output contains a single integer $m$ — the minimum number of sheets required.</p><p>Then $m$ lines follow: the $j$-th of these lines contains a string of two uppercase letters of the English alphabet — the letters appearing on the two sides of the $j$-th sheet.</p><p>Note that you can print the sheets and the two letters of each sheet in any order.</p></div>

## Input

<p>The first line contains a string $t$ consisting of uppercase letters of the English alphabet ($1\le |t| \le 1000$) — the name of the teddy bear.</p><p>The second line contains a string $o$ consisting of uppercase letters of the English alphabet ($1\le |o| \le 1000$) — the name of the owl.</p><p>The third line contains a string $r$ consisting of uppercase letters of the English alphabet ($1\le |r| \le 1000$) — the name of the raccoon.</p><p>The values $|t|$, $|o|$, $|r|$ denote the length of the three names $t$, $o$, $r$.</p>

## Output

<p>The first line of the output contains a single integer $m$ — the minimum number of sheets required.</p><p>Then $m$ lines follow: the $j$-th of these lines contains a string of two uppercase letters of the English alphabet — the letters appearing on the two sides of the $j$-th sheet.</p><p>Note that you can print the sheets and the two letters of each sheet in any order.</p>





```input1
AA
GA
MA
```




```input2
TEDDY
HEDWIG
RACCOON
```




```input3
BDC
CAA
CE
```




```output1
2
AG
AM
```




```output2
8
AT
CH
CY
DG
DO
ER
IN
OW
```




```output3
4
AD
AE
BB
CC
```



## Note

<p>In the <span class="tex-font-style-bf">first sample</span>, the solution uses two sheets: the first sheet has <span class="tex-font-style-tt">A</span> on one side and <span class="tex-font-style-tt">G</span> on the other side; the second sheet has <span class="tex-font-style-tt">A</span> on one side and <span class="tex-font-style-tt">M</span> on the other side.</p><p>The name <span class="tex-font-style-tt">AA</span> can be spelled using the <span class="tex-font-style-tt">A</span> side of both sheets. The name <span class="tex-font-style-tt">GA</span> can be spelled using the <span class="tex-font-style-tt">G</span> side of the first sheet and the <span class="tex-font-style-tt">A</span> side of the second sheet. Finally, the name <span class="tex-font-style-tt">MA</span> can be spelled using the <span class="tex-font-style-tt">M</span> side of the second sheet and the <span class="tex-font-style-tt">A</span> side of the first sheet.</p>
