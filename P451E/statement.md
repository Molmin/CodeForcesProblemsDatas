## Description

<div><p>Devu wants to decorate his garden with flowers. He has purchased <span class="tex-span"><i>n</i></span> boxes, where the <span class="tex-span"><i>i</i></span>-th box contains <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> flowers. All flowers in a single box are of the same color (hence they are indistinguishable). Also, no two boxes have flowers of the same color.</p><p>Now Devu wants to select <span class="tex-font-style-bf">exactly</span> <span class="tex-span"><i>s</i></span> flowers from the boxes to decorate his garden. Devu would like to know, in how many different ways can he select the flowers from each box? Since this number may be very large, he asks you to find the number modulo <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>. </p><p>Devu considers two ways different if there is at least one box from which different number of flowers are selected in these two ways.</p></div><div class="input-specification"><p>The first line of input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 20</span>, <span class="tex-span">0 ≤ <i>s</i> ≤ 10<sup class="upper-index">14</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>f</i><sub class="lower-index">1</sub>, <i>f</i><sub class="lower-index">2</sub>, ... <i>f</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">12</sup></span>).</p></div><div class="output-specification"><p>Output a single integer — the number of ways in which Devu can select the flowers modulo <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line of input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 20</span>, <span class="tex-span">0 ≤ <i>s</i> ≤ 10<sup class="upper-index">14</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>f</i><sub class="lower-index">1</sub>, <i>f</i><sub class="lower-index">2</sub>, ... <i>f</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">12</sup></span>).</p>

## Output

<p>Output a single integer — the number of ways in which Devu can select the flowers modulo <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
2 3
1 3

```




```input2
2 4
2 2

```




```input3
3 5
1 3 2

```




```output1
2

```




```output2
1

```




```output3
3

```



## Note

<p>Sample 1. There are two ways of selecting <span class="tex-span">3</span> flowers: <span class="tex-span">{1, 2}</span> and <span class="tex-span">{0, 3}</span>.</p><p>Sample 2. There is only one way of selecting <span class="tex-span">4</span> flowers: <span class="tex-span">{2, 2}</span>.</p><p>Sample 3. There are three ways of selecting <span class="tex-span">5</span> flowers: <span class="tex-span">{1, 2, 2}</span>, <span class="tex-span">{0, 3, 2}</span>, and <span class="tex-span">{1, 3, 1}</span>.</p>
