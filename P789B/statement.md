## Description

<div><p>Masha really loves algebra. On the last lesson, her strict teacher Dvastan gave she new exercise.</p><p>You are given geometric progression <span class="tex-span"><i>b</i></span> defined by two integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>q</i></span>. Remind that a geometric progression is a sequence of integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, <i>b</i><sub class="lower-index">3</sub>, ...</span>, where for each <span class="tex-span"><i>i</i> &gt; 1</span> the respective term satisfies the condition <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> = <i>b</i><sub class="lower-index"><i>i</i> - 1</sub>·<i>q</i></span>, where <span class="tex-span"><i>q</i></span> is called the common ratio of the progression. Progressions in Uzhlyandia are unusual: both <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>q</i></span> <span class="tex-font-style-bf">can equal <span class="tex-span">0</span></span>. Also, Dvastan gave Masha <span class="tex-span"><i>m</i></span> "bad" integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span>, and an integer <span class="tex-span"><i>l</i></span>.</p><p>Masha writes all progression terms one by one onto the board (including repetitive) while condition <span class="tex-span">|<i>b</i><sub class="lower-index"><i>i</i></sub>| ≤ <i>l</i></span> is satisfied (<span class="tex-span">|<i>x</i>|</span> means absolute value of <span class="tex-span"><i>x</i></span>). There is an exception: if a term equals one of the "bad" integers, Masha skips it (doesn't write onto the board) and moves forward to the next term.</p><p>But the lesson is going to end soon, so Masha has to calculate how many integers will be written on the board. In order not to get into depression, Masha asked you for help: help her calculate how many numbers she will write, or print "<span class="tex-font-style-tt">inf</span>" in case she needs to write infinitely many integers.</p></div><div class="input-specification"><p>The first line of input contains four integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>q</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>m</i></span> (-<span class="tex-span">10<sup class="upper-index">9</sup> ≤ <i>b</i><sub class="lower-index">1</sub>, <i>q</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>l</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the initial term and the common ratio of progression, absolute value of maximal number that can be written on the board and the number of "bad" integers, respectively.</p><p>The second line contains <span class="tex-span"><i>m</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span> (-<span class="tex-span">10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>&nbsp;— numbers that will never be written on the board.</p></div><div class="output-specification"><p>Print the only integer, meaning the number of progression terms that will be written on the board if it is finite, or "<span class="tex-font-style-tt">inf</span>" (without quotes) otherwise.</p></div>

## Input

<p>The first line of input contains four integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>q</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>m</i></span> (-<span class="tex-span">10<sup class="upper-index">9</sup> ≤ <i>b</i><sub class="lower-index">1</sub>, <i>q</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>l</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the initial term and the common ratio of progression, absolute value of maximal number that can be written on the board and the number of "bad" integers, respectively.</p><p>The second line contains <span class="tex-span"><i>m</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span> (-<span class="tex-span">10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>&nbsp;— numbers that will never be written on the board.</p>

## Output

<p>Print the only integer, meaning the number of progression terms that will be written on the board if it is finite, or "<span class="tex-font-style-tt">inf</span>" (without quotes) otherwise.</p>





```input1
3 2 30 4
6 14 25 48

```




```input2
123 1 2143435 4
123 11 -5453 141245

```




```input3
123 1 2143435 4
54343 -13 6 124

```




```output1
3
```




```output2
0
```




```output3
inf
```



## Note

<p>In the first sample case, Masha will write integers <span class="tex-span">3, 12, 24</span>. Progression term <span class="tex-span">6</span> will be skipped because it is a "bad" integer. Terms bigger than <span class="tex-span">24</span> won't be written because they exceed <span class="tex-span"><i>l</i></span> by absolute value.</p><p>In the second case, Masha won't write any number because all terms are equal <span class="tex-span">123</span> and this is a "bad" integer.</p><p>In the third case, Masha will write infinitely integers <span class="tex-span">123</span>. </p>
