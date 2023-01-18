## Description

<div><p>There are $n$ chips arranged in a circle, numbered from $1$ to $n$. </p><p>Initially each chip has black or white color. Then $k$ iterations occur. During each iteration the chips change their colors according to the following rules. For each chip $i$, three chips are considered: chip $i$ itself and two its neighbours. If the number of white chips among these three is greater than the number of black chips among these three chips, then the chip $i$ becomes white. Otherwise, the chip $i$ becomes black. </p><p>Note that for each $i$ from $2$ to $(n - 1)$ two neighbouring chips have numbers $(i - 1)$ and $(i + 1)$. The neighbours for the chip $i = 1$ are $n$ and $2$. The neighbours of $i = n$ are $(n - 1)$ and $1$.</p><p>The following picture describes one iteration with $n = 6$. The chips $1$, $3$ and $4$ are initially black, and the chips $2$, $5$ and $6$ are white. After the iteration $2$, $3$ and $4$ become black, and $1$, $5$ and $6$ become white.</p><center> <img class="tex-graphics" src="file://RBsgCbj4.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Your task is to determine the color of each chip after $k$ iterations.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ $(3 \le n \le 200\,000, 1 \le k \le 10^{9})$ — the number of chips and the number of iterations, respectively.</p><p>The second line contains a string consisting of $n$ characters "<span class="tex-font-style-tt">W</span>" and "<span class="tex-font-style-tt">B</span>". If the $i$-th character is "<span class="tex-font-style-tt">W</span>", then the $i$-th chip is white initially. If the $i$-th character is "<span class="tex-font-style-tt">B</span>", then the $i$-th chip is black initially.</p></div><div class="output-specification"><p>Print a string consisting of $n$ characters "<span class="tex-font-style-tt">W</span>" and "<span class="tex-font-style-tt">B</span>". If after $k$ iterations the $i$-th chip is white, then the $i$-th character should be "<span class="tex-font-style-tt">W</span>". Otherwise the $i$-th character should be "<span class="tex-font-style-tt">B</span>".</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ $(3 \le n \le 200\,000, 1 \le k \le 10^{9})$ — the number of chips and the number of iterations, respectively.</p><p>The second line contains a string consisting of $n$ characters "<span class="tex-font-style-tt">W</span>" and "<span class="tex-font-style-tt">B</span>". If the $i$-th character is "<span class="tex-font-style-tt">W</span>", then the $i$-th chip is white initially. If the $i$-th character is "<span class="tex-font-style-tt">B</span>", then the $i$-th chip is black initially.</p>

## Output

<p>Print a string consisting of $n$ characters "<span class="tex-font-style-tt">W</span>" and "<span class="tex-font-style-tt">B</span>". If after $k$ iterations the $i$-th chip is white, then the $i$-th character should be "<span class="tex-font-style-tt">W</span>". Otherwise the $i$-th character should be "<span class="tex-font-style-tt">B</span>".</p>





```input1
6 1
BWBBWW
```




```input2
7 3
WBWBWBW
```




```input3
6 4
BWBWBW
```




```output1
WBBBWW
```




```output2
WWWWWWW
```




```output3
BWBWBW
```



## Note

<p>The first example is described in the statement.</p><p>The second example: "<span class="tex-font-style-tt">WBWBWBW</span>" $\rightarrow$ "<span class="tex-font-style-tt">WWBWBWW</span>" $\rightarrow$ "<span class="tex-font-style-tt">WWWBWWW</span>" $\rightarrow$ "<span class="tex-font-style-tt">WWWWWWW</span>". So all chips become white.</p><p>The third example: "<span class="tex-font-style-tt">BWBWBW</span>" $\rightarrow$ "<span class="tex-font-style-tt">WBWBWB</span>" $\rightarrow$ "<span class="tex-font-style-tt">BWBWBW</span>" $\rightarrow$ "<span class="tex-font-style-tt">WBWBWB</span>" $\rightarrow$ "<span class="tex-font-style-tt">BWBWBW</span>".</p>
