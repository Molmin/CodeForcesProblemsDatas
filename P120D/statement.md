## Description

<div><p>Three sons inherited from their father a rectangular corn fiend divided into <span class="tex-span"><i>n</i> × <i>m</i></span> squares. For each square we know how many tons of corn grows on it. The father, an old farmer did not love all three sons equally, which is why he bequeathed to divide his field into three parts containing <span class="tex-span"><i>A</i></span>, <span class="tex-span"><i>B</i></span> and <span class="tex-span"><i>C</i></span> tons of corn.</p><p>The field should be divided by two parallel lines. The lines should be parallel to one side of the field and to each other. The lines should go strictly between the squares of the field. Each resulting part of the field should consist of at least one square. </p><p>Your task is to find the number of ways to divide the field as is described above, that is, to mark two lines, dividing the field in three parts so that on one of the resulting parts grew <span class="tex-span"><i>A</i></span> tons of corn, <span class="tex-span"><i>B</i></span> on another one and <span class="tex-span"><i>C</i></span> on the remaining one.</p></div><div class="input-specification"><p>The first line contains space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> — the sizes of the original (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 50, <i>max</i>(<i>n</i>, <i>m</i>) ≥ 3</span>). Then the field's description follows: <span class="tex-span"><i>n</i></span> lines, each containing <span class="tex-span"><i>m</i></span> space-separated integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>ij</i></sub></span>, (<span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>ij</i></sub> ≤ 100</span>) — the number of tons of corn each square contains. The last line contains space-separated integers <span class="tex-span"><i>A</i>, <i>B</i>, <i>C</i></span> (<span class="tex-span">0 ≤ <i>A</i>, <i>B</i>, <i>C</i> ≤ 10<sup class="upper-index">6</sup></span>).</p></div><div class="output-specification"><p>Print the answer to the problem: the number of ways to divide the father's field so that one of the resulting parts contained <span class="tex-span"><i>A</i></span> tons of corn, another one contained <span class="tex-span"><i>B</i></span> tons, and the remaining one contained <span class="tex-span"><i>C</i></span> tons. If no such way exists, print 0.</p></div>

## Input

<p>The first line contains space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> — the sizes of the original (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 50, <i>max</i>(<i>n</i>, <i>m</i>) ≥ 3</span>). Then the field's description follows: <span class="tex-span"><i>n</i></span> lines, each containing <span class="tex-span"><i>m</i></span> space-separated integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>ij</i></sub></span>, (<span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>ij</i></sub> ≤ 100</span>) — the number of tons of corn each square contains. The last line contains space-separated integers <span class="tex-span"><i>A</i>, <i>B</i>, <i>C</i></span> (<span class="tex-span">0 ≤ <i>A</i>, <i>B</i>, <i>C</i> ≤ 10<sup class="upper-index">6</sup></span>).</p>

## Output

<p>Print the answer to the problem: the number of ways to divide the father's field so that one of the resulting parts contained <span class="tex-span"><i>A</i></span> tons of corn, another one contained <span class="tex-span"><i>B</i></span> tons, and the remaining one contained <span class="tex-span"><i>C</i></span> tons. If no such way exists, print 0.</p>





```input1
3 3
1 1 1
1 1 1
1 1 1
3 3 3

```




```input2
2 5
1 1 1 1 1
2 2 2 2 2
3 6 6

```




```input3
3 3
1 2 3
3 1 2
2 3 1
5 6 7

```




```output1
2

```




```output2
3

```




```output3
0

```



## Note

<p>The lines dividing the field can be horizontal or vertical, but they should be parallel to each other.</p>
