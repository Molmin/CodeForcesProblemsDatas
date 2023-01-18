## Description

<div><p>There is a square painted on a piece of paper, the square's side equals <span class="tex-span"><i>n</i></span> meters. John Doe draws crosses on the square's perimeter. John paints the first cross in the lower left corner of the square. Then John moves along the square's perimeter in the clockwise direction (first upwards, then to the right, then downwards, then to the left and so on). Every time he walks <span class="tex-span">(<i>n</i> + 1)</span> meters, he draws a cross (see picture for clarifications).</p><p>John Doe stops only when the lower left corner of the square has two crosses. How many crosses will John draw?</p><center> <img class="tex-graphics" src="file://O5kIITk1.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-script"> The figure shows the order in which John draws crosses for a square with side <span class="tex-span">4</span>. The lower left square has two crosses. Overall John paints <span class="tex-span">17</span> crosses. </span> </center></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 10<sup class="upper-index">4</sup></span>) — the number of test cases. </p><p>The second line contains <span class="tex-span"><i>t</i></span> space-separated integers <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>n</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the sides of the square for each test sample.</p></div><div class="output-specification"><p>For each test sample print on a single line the answer to it, that is, the number of crosses John will draw as he will move along the square of the corresponding size. Print the answers to the samples in the order in which the samples are given in the input.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier. </p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 10<sup class="upper-index">4</sup></span>) — the number of test cases. </p><p>The second line contains <span class="tex-span"><i>t</i></span> space-separated integers <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>n</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the sides of the square for each test sample.</p>

## Output

<p>For each test sample print on a single line the answer to it, that is, the number of crosses John will draw as he will move along the square of the corresponding size. Print the answers to the samples in the order in which the samples are given in the input.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier. </p>





```input1
3
4 8 100

```




```output1
17
33
401

```


