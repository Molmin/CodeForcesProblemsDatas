## Description

<div><p>You have a stripe of checkered paper of length $n$. Each cell is either white or black.</p><p>What is the minimum number of cells that must be recolored from white to black in order to have a segment of $k$ consecutive black cells on the stripe?</p><p>If the input data is such that a segment of $k$ consecutive black cells already exists, then print <span class="tex-font-style-tt">0</span>. </p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>Next, descriptions of $t$ test cases follow.</p><p>The first line of the input contains two integers $n$ and $k$ ($1 \le k \le n \le 2\cdot10^5$). The second line consists of the letters '<span class="tex-font-style-tt">W</span>' (white) and '<span class="tex-font-style-tt">B</span>' (black). The line length is $n$.</p><p>It is guaranteed that the sum of values $n$ does not exceed $2\cdot10^5$.</p></div><div class="output-specification"><p>For each of $t$ test cases print an integer&nbsp;— the minimum number of cells that need to be repainted from white to black in order to have a segment of $k$ consecutive black cells.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>Next, descriptions of $t$ test cases follow.</p><p>The first line of the input contains two integers $n$ and $k$ ($1 \le k \le n \le 2\cdot10^5$). The second line consists of the letters '<span class="tex-font-style-tt">W</span>' (white) and '<span class="tex-font-style-tt">B</span>' (black). The line length is $n$.</p><p>It is guaranteed that the sum of values $n$ does not exceed $2\cdot10^5$.</p>

## Output

<p>For each of $t$ test cases print an integer&nbsp;— the minimum number of cells that need to be repainted from white to black in order to have a segment of $k$ consecutive black cells.</p>





```input1
4
5 3
BBWBW
5 5
BBWBW
5 1
BBWBW
1 1
W
```




```output1
1
2
0
1
```



## Note

<p>In the first test case, $s$="<span class="tex-font-style-tt">BBWBW</span>" and $k=3$. It is enough to recolor $s_3$ and get $s$="<span class="tex-font-style-tt">BBBBW</span>". This string contains a segment of length $k=3$ consisting of the letters '<span class="tex-font-style-tt">B</span>'.</p><p>In the second test case of the example $s$="<span class="tex-font-style-tt">BBWBW</span>" and $k=5$. It is enough to recolor $s_3$ and $s_5$ and get $s$="<span class="tex-font-style-tt">BBBBB</span>". This string contains a segment of length $k=5$ consisting of the letters '<span class="tex-font-style-tt">B</span>'.</p><p>In the third test case of the example $s$="<span class="tex-font-style-tt">BBWBW</span>" and $k=1$. The string $s$ already contains a segment of length $k=1$ consisting of the letters '<span class="tex-font-style-tt">B</span>'.</p>
