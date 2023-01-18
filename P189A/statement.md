## Description

<div><p>Polycarpus has a ribbon, its length is <span class="tex-span"><i>n</i></span>. He wants to cut the ribbon in a way that fulfils the following two conditions: </p><ul> <li> After the cutting each ribbon piece should have length <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> or <span class="tex-span"><i>c</i></span>. </li><li> After the cutting the number of ribbon pieces should be maximum. </li></ul><p>Help Polycarpus and find the number of ribbon pieces after the required cutting.</p></div><div class="input-specification"><p>The first line contains four space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>a</i>, <i>b</i>, <i>c</i> ≤ 4000)</span> — the length of the original ribbon and the acceptable lengths of the ribbon pieces after the cutting, correspondingly. The numbers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> can coincide.</p></div><div class="output-specification"><p>Print a single number — the maximum possible number of ribbon pieces. It is guaranteed that at least one correct ribbon cutting exists.</p></div>

## Input

<p>The first line contains four space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>a</i>, <i>b</i>, <i>c</i> ≤ 4000)</span> — the length of the original ribbon and the acceptable lengths of the ribbon pieces after the cutting, correspondingly. The numbers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> can coincide.</p>

## Output

<p>Print a single number — the maximum possible number of ribbon pieces. It is guaranteed that at least one correct ribbon cutting exists.</p>





```input1
5 5 3 2

```




```input2
7 5 5 2

```




```output1
2

```




```output2
2

```



## Note

<p>In the first example Polycarpus can cut the ribbon in such way: the first piece has length 2, the second piece has length 3.</p><p>In the second example Polycarpus can cut the ribbon in such way: the first piece has length 5, the second piece has length 2.</p>
