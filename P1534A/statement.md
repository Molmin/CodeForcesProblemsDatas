## Description

<div><p>Today we will be playing a red and white colouring game (no, this is not the Russian Civil War; these are just the colours of the Canadian flag).</p><p>You are given an $n \times m$ grid of "<span class="tex-font-style-tt">R</span>", "<span class="tex-font-style-tt">W</span>", and "<span class="tex-font-style-tt">.</span>" characters. "<span class="tex-font-style-tt">R</span>" is red, "<span class="tex-font-style-tt">W</span>" is white and "<span class="tex-font-style-tt">.</span>" is blank. The neighbours of a cell are those that share an edge with it (those that only share a corner do not count).</p><p>Your job is to colour the blank cells red or white so that every red cell only has white neighbours (and no red ones) and every white cell only has red neighbours (and no white ones). You are not allowed to recolour already coloured cells.</p></div><div class="input-specification"><p>The first line contains $t$ ($1 \le t \le 100$), the number of test cases.</p><p>In each test case, the first line will contain $n$ ($1 \le n \le 50$) and $m$ ($1 \le m \le 50$), the height and width of the grid respectively.</p><p>The next $n$ lines will contain the grid. Each character of the grid is either '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">W</span>', or '<span class="tex-font-style-tt">.</span>'.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">YES</span>" if there is a valid grid or "<span class="tex-font-style-tt">NO</span>" if there is not.</p><p>If there is, output the grid on the next $n$ lines. If there are multiple answers, print any.</p><p>In the output, the "<span class="tex-font-style-tt">YES</span>"s and "<span class="tex-font-style-tt">NO</span>"s are case-insensitive, meaning that outputs such as "<span class="tex-font-style-tt">yEs</span>" and "<span class="tex-font-style-tt">nO</span>" are valid. However, <span class="tex-font-style-bf">the grid is case-sensitive</span>.</p></div>

## Input

<p>The first line contains $t$ ($1 \le t \le 100$), the number of test cases.</p><p>In each test case, the first line will contain $n$ ($1 \le n \le 50$) and $m$ ($1 \le m \le 50$), the height and width of the grid respectively.</p><p>The next $n$ lines will contain the grid. Each character of the grid is either '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">W</span>', or '<span class="tex-font-style-tt">.</span>'.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">YES</span>" if there is a valid grid or "<span class="tex-font-style-tt">NO</span>" if there is not.</p><p>If there is, output the grid on the next $n$ lines. If there are multiple answers, print any.</p><p>In the output, the "<span class="tex-font-style-tt">YES</span>"s and "<span class="tex-font-style-tt">NO</span>"s are case-insensitive, meaning that outputs such as "<span class="tex-font-style-tt">yEs</span>" and "<span class="tex-font-style-tt">nO</span>" are valid. However, <span class="tex-font-style-bf">the grid is case-sensitive</span>.</p>





```input1
3
4 6
.R....
......
......
.W....
4 4
.R.W
....
....
....
5 1
R
W
R
W
R
```




```output1
YES
WRWRWR
RWRWRW
WRWRWR
RWRWRW
NO
YES
R
W
R
W
R
```



## Note

<p>The answer for the first example case is given in the example output, and it can be proven that no grid exists that satisfies the requirements of the second example case. In the third example all cells are initially coloured, and the colouring is valid.</p>
