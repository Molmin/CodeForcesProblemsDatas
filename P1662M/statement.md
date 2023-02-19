## Description

<div><p>Gabriella has been instructed to organize a renowned wine tasting event which will be attended by $m$ critics. On display, there will be $n$ different varieties of wine, each of which can either be a red wine or a white wine.</p><p>The wines will come in $n$ bottles arranged in a line on the table, and, for convenience, each critic will sip from a contiguous interval of bottles: that is, he/she will taste exactly the bottles at position $a, \, a + 1, \, \dots, \, b$ for some $1 \le a \le b \le n$. The interval depends on the critic, who will select it on the spot according to their preferences. In fact, the $i$-th critic ($1 \le i \le m$) has requested that he/she wants to taste exactly $r_i$ red wines and $w_i$ white wines.</p><p>Gabriella has yet to choose how many bottles of red wine and white wine there will be, and in what order they will appear. Help her find an arrangement (that is, a sequence of $n$ bottles of either red or white wine) that satisfies the requests of all the critics, or state that no such arrangement exists.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains an integer $t$ ($1\le t\le 100$) — the number of test cases. The descriptions of the $t$ test cases follow.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n \le 100$, $1 \le m \le 100$) — the number of bottles of wine and the number of critics.</p><p>Each of the next $m$ lines contains two integers $r_i$ and $w_i$ ($0 \le r_i, \, w_i \le 100$, $r_i + w_i \ge 1$) — the number of red and white wines that the $i$-th critic wants to taste.</p></div><div class="output-specification"><p>For each test case, if at least one solution exists, print a string of length $n$ made up of the characters <span class="tex-font-style-tt">R</span> and <span class="tex-font-style-tt">W</span>, where the $j$-th character ($1 \le j \le n$) denotes the type of the wine in the $j$-th bottle of the arrangement (<span class="tex-font-style-tt">R</span> for <span class="tex-font-style-it">red</span> and <span class="tex-font-style-tt">W</span> for <span class="tex-font-style-it">white</span>). If there are multiple solutions, print any.</p><p>If no solution exists, print the string <span class="tex-font-style-tt">IMPOSSIBLE</span>.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains an integer $t$ ($1\le t\le 100$) — the number of test cases. The descriptions of the $t$ test cases follow.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n \le 100$, $1 \le m \le 100$) — the number of bottles of wine and the number of critics.</p><p>Each of the next $m$ lines contains two integers $r_i$ and $w_i$ ($0 \le r_i, \, w_i \le 100$, $r_i + w_i \ge 1$) — the number of red and white wines that the $i$-th critic wants to taste.</p>

## Output

<p>For each test case, if at least one solution exists, print a string of length $n$ made up of the characters <span class="tex-font-style-tt">R</span> and <span class="tex-font-style-tt">W</span>, where the $j$-th character ($1 \le j \le n$) denotes the type of the wine in the $j$-th bottle of the arrangement (<span class="tex-font-style-tt">R</span> for <span class="tex-font-style-it">red</span> and <span class="tex-font-style-tt">W</span> for <span class="tex-font-style-it">white</span>). If there are multiple solutions, print any.</p><p>If no solution exists, print the string <span class="tex-font-style-tt">IMPOSSIBLE</span>.</p>





```input1|2,3,4,5,10,11,12
3
5 3
1 0
3 2
2 2
4 3
2 1
1 1
0 3
3 2
0 2
0 3
```




```output1
RWRRW
IMPOSSIBLE
WWW
```



## Note

<p>In the <span class="tex-font-style-bf">first test case</span>, there are $n = 5$ bottles of wine to be arranged and $m = 3$ critics. The arrangement <span class="tex-font-style-tt">RWRRW</span> satisfies the requests of all three critics. Indeed: </p><ul> <li> the first critic can choose the interval $[3, \, 3]$, which contains exactly one bottle of red wine (note that $[1, \, 1]$ and $[4, \, 4]$ are other valid choices); </li><li> the second critic can choose the interval $[1, \, 5]$, which contains $3$ bottles of red wine and $2$ bottles of white wine; </li><li> the third critic can choose the interval $[2, \, 5]$, which contains $2$ bottles of red wine and $2$ bottles of white wine. </li></ul>
