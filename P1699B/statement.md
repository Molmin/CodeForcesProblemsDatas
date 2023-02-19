## Description

<div><p>You are given two <span class="tex-font-style-bf">even</span> integers $n$ and $m$. Your task is to find <span class="tex-font-style-bf">any</span> binary matrix $a$ with $n$ rows and $m$ columns where every cell $(i,j)$ has <span class="tex-font-style-bf">exactly</span> two neighbours with a different value than $a_{i,j}$.</p><p>Two cells in the matrix are considered neighbours if and only if they share a side. More formally, the neighbours of cell $(x,y)$ are: $(x-1,y)$, $(x,y+1)$, $(x+1,y)$ and $(x,y-1)$.</p><p>It can be proven that under the given constraints, an answer always exists.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line of input contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases. The following lines contain the descriptions of the test cases.</p><p>The only line of each test case contains two <span class="tex-font-style-bf">even</span> integers $n$ and $m$ ($2 \le n,m \le 50$)&nbsp;— the height and width of the binary matrix, respectively.</p></div><div class="output-specification"><p>For each test case, print $n$ lines, each of which contains $m$ numbers, equal to $0$ or $1$&nbsp;— any binary matrix which satisfies the constraints described in the statement.</p><p>It can be proven that under the given constraints, an answer always exists.</p></div>

## Input

<p>Each test contains multiple test cases. The first line of input contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases. The following lines contain the descriptions of the test cases.</p><p>The only line of each test case contains two <span class="tex-font-style-bf">even</span> integers $n$ and $m$ ($2 \le n,m \le 50$)&nbsp;— the height and width of the binary matrix, respectively.</p>

## Output

<p>For each test case, print $n$ lines, each of which contains $m$ numbers, equal to $0$ or $1$&nbsp;— any binary matrix which satisfies the constraints described in the statement.</p><p>It can be proven that under the given constraints, an answer always exists.</p>





```input1|2,4
3
2 4
2 2
4 4
```




```output1
1 0 0 1
0 1 1 0
1 0
0 1
1 0 1 0
0 0 1 1
1 1 0 0
0 1 0 1
```



## Note

<p>White means $0$, black means $1$.</p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><img class="tex-graphics" src="file://gDTxL5GH.png" style="max-width: 100.0%;max-height: 100.0%;"></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><img class="tex-graphics" src="file://p7cPEf9a.png" style="max-width: 100.0%;max-height: 100.0%;"></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><img class="tex-graphics" src="file://qiKuVmbt.png" style="max-width: 100.0%;max-height: 100.0%;"></td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-size-small">The binary matrix from the first test case</span></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-size-small">The binary matrix from the second test case</span></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-size-small">The binary matrix from the third test case</span></td></tr></tbody></table> </center>
