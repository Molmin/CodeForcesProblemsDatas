## Description

<div><p>You are given an $n \times m$ table, consisting of characters «<span class="tex-font-style-tt">A</span>», «<span class="tex-font-style-tt">G</span>», «<span class="tex-font-style-tt">C</span>», «<span class="tex-font-style-tt">T</span>». Let's call a table <span class="tex-font-style-it">nice</span>, if every $2 \times 2$ square contains all four distinct characters. Your task is to find a nice table (also consisting of «<span class="tex-font-style-tt">A</span>», «<span class="tex-font-style-tt">G</span>», «<span class="tex-font-style-tt">C</span>», «<span class="tex-font-style-tt">T</span>»), that differs from the given table in the minimum number of characters.</p></div><div class="input-specification"><p>First line contains two positive integers $n$ and $m$&nbsp;— number of rows and columns in the table you are given ($2 \leq n, m, n \times m \leq 300\,000$). Then, $n$ lines describing the table follow. Each line contains exactly $m$ characters «<span class="tex-font-style-tt">A</span>», «<span class="tex-font-style-tt">G</span>», «<span class="tex-font-style-tt">C</span>», «<span class="tex-font-style-tt">T</span>».</p></div><div class="output-specification"><p>Output $n$ lines, $m$ characters each. This table must be nice and differ from the input table in the minimum number of characters.</p></div>

## Input

<p>First line contains two positive integers $n$ and $m$&nbsp;— number of rows and columns in the table you are given ($2 \leq n, m, n \times m \leq 300\,000$). Then, $n$ lines describing the table follow. Each line contains exactly $m$ characters «<span class="tex-font-style-tt">A</span>», «<span class="tex-font-style-tt">G</span>», «<span class="tex-font-style-tt">C</span>», «<span class="tex-font-style-tt">T</span>».</p>

## Output

<p>Output $n$ lines, $m$ characters each. This table must be nice and differ from the input table in the minimum number of characters.</p>





```input1
2 2
AG
CT
```




```input2
3 5
AGCAG
AGCAG
AGCAG
```




```output1
AG
CT
```




```output2
TGCAT
CATGC
TGCAT
```



## Note

<p>In the first sample, the table is already nice. In the second sample, you can change 9 elements to make the table nice.</p>
