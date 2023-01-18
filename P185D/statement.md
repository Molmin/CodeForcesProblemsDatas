## Description

<div><p>The Great Mushroom King descended to the dwarves, but not everyone managed to see him. Only the few chosen ones could see the King.</p><p>We know that only <span class="tex-span"><i>LCM</i>(<i>k</i><sup class="upper-index">2<sup class="upper-index"><i>l</i></sup></sup> + 1, <i>k</i><sup class="upper-index">2<sup class="upper-index"><i>l</i> + 1</sup></sup> + 1, ..., <i>k</i><sup class="upper-index">2<sup class="upper-index"><i>r</i></sup></sup> + 1)</span> dwarves can see the Great Mushroom King. Numbers <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> are chosen by the Great Mushroom King himself in some complicated manner which is unclear to common dwarves. </p><p>The dwarven historians decided to document all visits of the Great Mushroom King. For each visit the dwarven historians know three integers <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, chosen by the Great Mushroom King for this visit. They also know a prime number <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>. Help them to count the remainder of dividing the number of dwarves who can see the King, by number <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, for each visit.</p></div><div class="input-specification"><p>The first line contains the single integer <span class="tex-span"><i>t</i></span> <span class="tex-span">(1 ≤ <i>t</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of the King's visits. </p><p>Each of the following <span class="tex-span"><i>t</i></span> input lines contains four space-separated integers <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>;&nbsp;<span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup>;&nbsp;2 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — the numbers, chosen by the Great Mushroom King and the prime module, correspondingly. </p><p>It is guaranteed that for all visits number <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is prime.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div><div class="output-specification"><p>For each visit print the answer on a single line — the remainder of dividing the number of the dwarves who can see the King this time, by number <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>. Print the answers for the visits in the order, in which the visits are described in the input.</p></div>

## Input

<p>The first line contains the single integer <span class="tex-span"><i>t</i></span> <span class="tex-span">(1 ≤ <i>t</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of the King's visits. </p><p>Each of the following <span class="tex-span"><i>t</i></span> input lines contains four space-separated integers <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>;&nbsp;<span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup>;&nbsp;2 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — the numbers, chosen by the Great Mushroom King and the prime module, correspondingly. </p><p>It is guaranteed that for all visits number <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is prime.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>

## Output

<p>For each visit print the answer on a single line — the remainder of dividing the number of the dwarves who can see the King this time, by number <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>. Print the answers for the visits in the order, in which the visits are described in the input.</p>





```input1
2
3 1 10 2
5 0 4 3

```




```output1
0
0

```



## Note

<p>We consider that <span class="tex-span"><i>LCM</i>(<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>)</span> represents the least common multiple of numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span>.</p><p>We consider that <span class="tex-span"><i>x</i><sup class="upper-index">0</sup> = 1</span>, for any <span class="tex-span"><i>x</i></span>.</p>
