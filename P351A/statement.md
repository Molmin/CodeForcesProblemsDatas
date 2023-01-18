## Description

<div><p>Jeff got <span class="tex-span">2<i>n</i></span> real numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index">2<i>n</i></sub></span> as a birthday present. The boy hates non-integer numbers, so he decided to slightly "adjust" the numbers he's got. Namely, Jeff consecutively executes <span class="tex-span"><i>n</i></span> operations, each of them goes as follows:</p><ul> <li> choose indexes <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> <span class="tex-span">(<i>i</i> ≠ <i>j</i>)</span> that haven't been chosen yet; </li><li> round element <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to the nearest integer that isn't more than <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (assign to <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>: <span class="tex-span">⌊ <i>a</i><sub class="lower-index"><i>i</i></sub>&nbsp;⌋</span>); </li><li> round element <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> to the nearest integer that isn't less than <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> (assign to <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span>: <span class="tex-span">⌈ <i>a</i><sub class="lower-index"><i>j</i></sub>&nbsp;⌉</span>). </li></ul><p>Nevertheless, Jeff doesn't want to hurt the feelings of the person who gave him the sequence. That's why the boy wants to perform the operations so as to make the absolute value of the difference between the sum of elements before performing the operations and the sum of elements after performing the operations as small as possible. Help Jeff find the minimum absolute value of the difference.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 2000)</span>. The next line contains <span class="tex-span">2<i>n</i></span> real numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index">2<i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10000)</span>, given with exactly three digits after the decimal point. The numbers are separated by spaces.</p></div><div class="output-specification"><p>In a single line print a single real number — the required difference with <span class="tex-font-style-bf">exactly three digits</span> after the decimal point.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 2000)</span>. The next line contains <span class="tex-span">2<i>n</i></span> real numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index">2<i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10000)</span>, given with exactly three digits after the decimal point. The numbers are separated by spaces.</p>

## Output

<p>In a single line print a single real number — the required difference with <span class="tex-font-style-bf">exactly three digits</span> after the decimal point.</p>





```input1
3
0.000 0.500 0.750 1.000 2.000 3.000

```




```input2
3
4469.000 6526.000 4864.000 9356.383 7490.000 995.896

```




```output1
0.250

```




```output2
0.279

```



## Note

<p>In the first test case you need to perform the operations as follows: <span class="tex-span">(<i>i</i> = 1, <i>j</i> = 4)</span>, <span class="tex-span">(<i>i</i> = 2, <i>j</i> = 3)</span>, <span class="tex-span">(<i>i</i> = 5, <i>j</i> = 6)</span>. In this case, the difference will equal <span class="tex-span">|(0 + 0.5 + 0.75 + 1 + 2 + 3) - (0 + 0 + 1 + 1 + 2 + 3)| = 0.25</span>. </p>
