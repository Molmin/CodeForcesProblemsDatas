## Description

<div><p>It is known that passages in Singer house are complex and intertwined. Let's define a Singer <span class="tex-span"><i>k</i></span>-house as a graph built by the following process: take complete binary tree of height <span class="tex-span"><i>k</i></span> and add edges from each vertex to all its successors, if they are not yet present.</p><center> <img class="tex-graphics" height="265px" src="file://WMH6D7yu.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px"> <span class="tex-font-size-small">Singer <span class="tex-span">4</span>-house</span> </center><p>Count the number of non-empty paths in Singer <span class="tex-span"><i>k</i></span>-house which do not pass the same vertex twice. Two paths are distinct if the sets or the orders of visited vertices are different. Since the answer can be large, output it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The only line contains single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 400</span>).</p></div><div class="output-specification"><p>Print single integer&nbsp;— the answer for the task modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The only line contains single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 400</span>).</p>

## Output

<p>Print single integer&nbsp;— the answer for the task modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
2

```




```input2
3

```




```input3
20

```




```output1
9

```




```output2
245

```




```output3
550384565

```



## Note

<p>There are <span class="tex-span">9</span> paths in the first example (the vertices are numbered on the picture below): <span class="tex-font-style-tt">1</span>, <span class="tex-font-style-tt">2</span>, <span class="tex-font-style-tt">3</span>, <span class="tex-font-style-tt">1-2</span>, <span class="tex-font-style-tt">2-1</span>, <span class="tex-font-style-tt">1-3</span>, <span class="tex-font-style-tt">3-1</span>, <span class="tex-font-style-tt">2-1-3</span>, <span class="tex-font-style-tt">3-1-2</span>.</p><center> <img class="tex-graphics" height="95px" src="file://IyycDlLN.png" style="max-width: 100.0%;max-height: 100.0%;" width="227px"> <span class="tex-font-size-small">Singer <span class="tex-span">2</span>-house</span> </center>
