## Description

<div><p>Levko loves tables that consist of <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>n</i></span> columns very much. He especially loves beautiful tables. A table is <span class="tex-font-style-it">beautiful</span> to Levko if the sum of elements in each row and column of the table equals <span class="tex-span"><i>k</i></span>.</p><p>Unfortunately, he doesn't know any such table. Your task is to help him to find at least one of them. </p></div><div class="input-specification"><p>The single line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 1000</span>).</p></div><div class="output-specification"><p>Print any beautiful table. Levko doesn't like too big numbers, so all elements of the table mustn't exceed <span class="tex-span">1000</span> in their absolute value.</p><p>If there are multiple suitable tables, you are allowed to print any of them.</p></div>

## Input

<p>The single line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 1000</span>).</p>

## Output

<p>Print any beautiful table. Levko doesn't like too big numbers, so all elements of the table mustn't exceed <span class="tex-span">1000</span> in their absolute value.</p><p>If there are multiple suitable tables, you are allowed to print any of them.</p>





```input1
2 4

```




```input2
4 7

```




```output1
1 3
3 1

```




```output2
2 1 0 4
4 0 2 1
1 3 3 0
0 3 2 2

```



## Note

<p>In the first sample the sum in the first row is <span class="tex-span">1 + 3 = 4</span>, in the second row — <span class="tex-span">3 + 1 = 4</span>, in the first column — <span class="tex-span">1 + 3 = 4</span> and in the second column — <span class="tex-span">3 + 1 = 4</span>. There are other beautiful tables for this sample.</p><p>In the second sample the sum of elements in each row and each column equals <span class="tex-span">7</span>. Besides, there are other tables that meet the statement requirements.</p>
