## Description

<div><p>We know that lucky digits are digits <span class="tex-span">4</span> and <span class="tex-span">7</span>, however Vasya's got another favorite digit <span class="tex-span">0</span> and he assumes it also is lucky! Lucky numbers are such <span class="tex-font-style-bf">non-negative</span> integers whose decimal record only contains lucky digits. For example, numbers <span class="tex-span">0, 47, 7074</span> are lucky, but <span class="tex-span">1, 7377, 895, </span> -<span class="tex-span">7</span> are not.</p><p>Vasya has <span class="tex-span"><i>t</i></span> important positive integers he needs to remember. Vasya is quite superstitious and he wants to remember lucky numbers only, so he is asking you for each important number to represent it as a sum of exactly six lucky numbers (Vasya just can't remember more numbers). Then Vasya can just remember these six numbers and calculate the important number at any moment.</p><p>For each of <span class="tex-span"><i>t</i></span> important integers represent it as the sum of six lucky numbers or state that this is impossible.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>t</i></span> <span class="tex-span">(1 ≤ <i>t</i> ≤ 5000)</span>.</p><p>Next <span class="tex-span"><i>t</i></span> lines contain a single positive integer <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>n</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup>)</span> — the list of important numbers.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> to read or write 64-bit integers С++. It is preferred to read the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>t</i></span> lines. The <span class="tex-span"><i>i</i></span>-th line must contain the answer for the <span class="tex-span"><i>i</i></span>-th important number: if the solution exists, the line must contain exactly six lucky numbers the sum of which equals <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span>, if the solution doesn't exist the string must contain a single integer <span class="tex-font-style-tt">-1</span>.</p><p>If there are multiple answers print any of them.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>t</i></span> <span class="tex-span">(1 ≤ <i>t</i> ≤ 5000)</span>.</p><p>Next <span class="tex-span"><i>t</i></span> lines contain a single positive integer <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>n</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup>)</span> — the list of important numbers.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> to read or write 64-bit integers С++. It is preferred to read the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>

## Output

<p>Print <span class="tex-span"><i>t</i></span> lines. The <span class="tex-span"><i>i</i></span>-th line must contain the answer for the <span class="tex-span"><i>i</i></span>-th important number: if the solution exists, the line must contain exactly six lucky numbers the sum of which equals <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span>, if the solution doesn't exist the string must contain a single integer <span class="tex-font-style-tt">-1</span>.</p><p>If there are multiple answers print any of them.</p>





```input1
5
42
17
444
7
51

```




```output1
7 7 7 7 7 7
-1
400 0 40 0 4 0
7 0 0 0 0 0
47 4 0 0 0 0

```


