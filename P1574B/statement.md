## Description

<div><p>You are given four integer values $a$, $b$, $c$ and $m$.</p><p>Check if there exists a string that contains: </p><ul> <li> $a$ letters '<span class="tex-font-style-tt">A</span>'; </li><li> $b$ letters '<span class="tex-font-style-tt">B</span>'; </li><li> $c$ letters '<span class="tex-font-style-tt">C</span>'; </li><li> no other letters; </li><li> exactly $m$ pairs of adjacent equal letters (exactly $m$ such positions $i$ that the $i$-th letter is equal to the $(i+1)$-th one). </li></ul></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>Each of the next $t$ lines contains the description of the testcase&nbsp;— four integers $a$, $b$, $c$ and $m$ ($1 \le a, b, c \le 10^8$; $0 \le m \le 10^8$).</p></div><div class="output-specification"><p>For each testcase print "<span class="tex-font-style-tt">YES</span>" if there exists a string that satisfies all the requirements. Print "<span class="tex-font-style-tt">NO</span>" if there are no such strings.</p><p>You may print every letter in any case you want (so, for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will all be recognized as positive answer).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>Each of the next $t$ lines contains the description of the testcase&nbsp;— four integers $a$, $b$, $c$ and $m$ ($1 \le a, b, c \le 10^8$; $0 \le m \le 10^8$).</p>

## Output

<p>For each testcase print "<span class="tex-font-style-tt">YES</span>" if there exists a string that satisfies all the requirements. Print "<span class="tex-font-style-tt">NO</span>" if there are no such strings.</p><p>You may print every letter in any case you want (so, for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will all be recognized as positive answer).</p>





```input1
3
2 2 1 0
1 1 1 1
1 2 3 2
```




```output1
YES
NO
YES
```



## Note

<p>In the first testcase strings "<span class="tex-font-style-tt">ABCAB</span>" or "<span class="tex-font-style-tt">BCABA</span>" satisfy the requirements. There exist other possible strings.</p><p>In the second testcase there's no way to put adjacent equal letters if there's no letter that appears at least twice.</p><p>In the third testcase string "<span class="tex-font-style-tt">CABBCC</span>" satisfies the requirements. There exist other possible strings.</p>
