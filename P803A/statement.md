## Description

<div><p>You are given matrix with <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>n</i></span> columns filled with zeroes. You should put <span class="tex-span"><i>k</i></span> ones in it in such a way that the resulting matrix is symmetrical with respect to the main diagonal (the diagonal that goes from the top left to the bottom right corner) and is lexicographically maximal.</p><p>One matrix is lexicographically greater than the other if the first different number in the first different row from the top in the first matrix is greater than the corresponding number in the second one.</p><p>If there exists no such matrix then output <span class="tex-font-style-tt">-1</span>.</p></div><div class="input-specification"><p>The first line consists of two numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">6</sup></span>).</p></div><div class="output-specification"><p>If the answer exists then output resulting matrix. Otherwise output <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line consists of two numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">6</sup></span>).</p>

## Output

<p>If the answer exists then output resulting matrix. Otherwise output <span class="tex-font-style-tt">-1</span>.</p>





```input1
2 1

```




```input2
3 2

```




```input3
2 5

```




```output1
1 0 
0 0 

```




```output2
1 0 0 
0 1 0 
0 0 0 

```




```output3
-1

```


