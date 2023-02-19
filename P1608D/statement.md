## Description

<div><p>You are given $n$ dominoes. Each domino has a left and a right cell. Each cell can be colored either black or white. Some cells are already colored, while some aren't yet.</p><p>The coloring is said to be <span class="tex-font-style-bf">valid</span> if and only if it is possible to rearrange the dominoes in some order such that for each $1 \le i \le n$ the color of the right cell of the $i$-th domino is different from the color of the left cell of the $((i \bmod n)+1)$-st domino. </p><p>Note that you can't rotate the dominoes, so the left cell always remains the left cell, and the right cell always remains the right cell.</p><p>Count the number of valid ways to color the yet uncolored cells of dominoes. Two ways are considered different if there is a cell that is colored white in one way and black in the other. In particular, colorings <span class="tex-font-style-tt">BW</span> <span class="tex-font-style-tt">WB</span> and <span class="tex-font-style-tt">WB</span> <span class="tex-font-style-tt">BW</span> different (and both invalid).</p><p>As this number can be very big, output it modulo $998\,244\,353$.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $n$ ($1 \le n \le 10^5$) — the number of dominoes.</p><p>The next $n$ lines describe dominoes. Each line contains two characters which represent the left and the right cell. Character <span class="tex-font-style-tt">B</span> means that the corresponding cell is black, character <span class="tex-font-style-tt">W</span> means that the corresponding cell is white, and <span class="tex-font-style-tt">?</span> means that the cell is yet to be colored. </p></div><div class="output-specification"><p>Print a single integer — the answer to the problem.</p></div>

## Input

<p>The first line of the input contains a single integer $n$ ($1 \le n \le 10^5$) — the number of dominoes.</p><p>The next $n$ lines describe dominoes. Each line contains two characters which represent the left and the right cell. Character <span class="tex-font-style-tt">B</span> means that the corresponding cell is black, character <span class="tex-font-style-tt">W</span> means that the corresponding cell is white, and <span class="tex-font-style-tt">?</span> means that the cell is yet to be colored. </p>

## Output

<p>Print a single integer — the answer to the problem.</p>





```input1
1
?W
```




```input2
2
??
W?
```




```input3
4
BB
??
W?
??
```




```output1
1
```




```output2
2
```




```output3
10
```



## Note

<p>In the first test case, there is only one domino, and we need the color of its right cell to be different from the color of its left cell. There is only one way to achieve this.</p><p>In the second test case, there are only $2$ such colorings:</p><p><span class="tex-font-style-tt">BB</span> <span class="tex-font-style-tt">WW</span> and <span class="tex-font-style-tt">WB</span> <span class="tex-font-style-tt">WB</span>.</p>
