## Description

<div><p>Boris really likes numbers and even owns a small shop selling interesting numbers. He has <span class="tex-span"><i>n</i></span> decimal numbers <span class="tex-span"><i>B</i><sub class="lower-index"><i>i</i></sub></span>. Cost of the number in his shop is equal to the sum of costs of its digits. You are given the values <span class="tex-span"><i>c</i><sub class="lower-index"><i>d</i></sub></span>, where <span class="tex-span"><i>c</i><sub class="lower-index"><i>d</i></sub></span> is the cost of the digit <span class="tex-span"><i>d</i></span>. Of course, Boris is interested in that numbers he owns have the maximum cost possible.</p><p>Recently Boris got hold of the magical artifact <span class="tex-span"><i>A</i></span>, which can allow him to increase the cost of his collection. Artifact is a string, consisting of digits and '<span class="tex-font-style-tt">?</span>' symbols. To use the artifact, Boris must replace all '<span class="tex-font-style-tt">?</span>' with digits to get a decimal number without leading zeros (it is also not allowed to get number 0). After that, the resulting number is added to all numbers <span class="tex-span"><i>B</i><sub class="lower-index"><i>i</i></sub></span> in Boris' collection. He uses the artifact exactly once.</p><p>What is the maximum cost of the collection Boris can achieve after using the artifact?</p></div><div class="input-specification"><p>First line contains artifact <span class="tex-span"><i>A</i></span>, consisting of digits '<span class="tex-font-style-tt">0</span>'–'<span class="tex-font-style-tt">9</span>' and '<span class="tex-font-style-tt">?</span>' symbols (<span class="tex-span">1 ≤ |<i>A</i>| ≤ 1000</span>). Next line contains <span class="tex-span"><i>n</i></span>&nbsp;— the amount of numbers in Boris' collection (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>). Next <span class="tex-span"><i>n</i></span> lines contain integers <span class="tex-span"><i>B</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>B</i><sub class="lower-index"><i>i</i></sub> &lt; 10<sup class="upper-index">1000</sup></span>). <span class="tex-span"><i>A</i></span> doesn't start with '<span class="tex-font-style-tt">0</span>'.</p><p>Last line contains ten integers&nbsp;— costs of digits <span class="tex-span"><i>c</i><sub class="lower-index">0</sub>, <i>c</i><sub class="lower-index">1</sub>, ..., <i>c</i><sub class="lower-index">9</sub></span> (<span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>).</p></div><div class="output-specification"><p>Output one integer&nbsp;— the maximum possible cost of the collection after using the artifact.</p></div>

## Input

<p>First line contains artifact <span class="tex-span"><i>A</i></span>, consisting of digits '<span class="tex-font-style-tt">0</span>'–'<span class="tex-font-style-tt">9</span>' and '<span class="tex-font-style-tt">?</span>' symbols (<span class="tex-span">1 ≤ |<i>A</i>| ≤ 1000</span>). Next line contains <span class="tex-span"><i>n</i></span>&nbsp;— the amount of numbers in Boris' collection (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>). Next <span class="tex-span"><i>n</i></span> lines contain integers <span class="tex-span"><i>B</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>B</i><sub class="lower-index"><i>i</i></sub> &lt; 10<sup class="upper-index">1000</sup></span>). <span class="tex-span"><i>A</i></span> doesn't start with '<span class="tex-font-style-tt">0</span>'.</p><p>Last line contains ten integers&nbsp;— costs of digits <span class="tex-span"><i>c</i><sub class="lower-index">0</sub>, <i>c</i><sub class="lower-index">1</sub>, ..., <i>c</i><sub class="lower-index">9</sub></span> (<span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>).</p>

## Output

<p>Output one integer&nbsp;— the maximum possible cost of the collection after using the artifact.</p>





```input1
42
3
89
1
958
0 0 1 1 2 2 3 3 4 4

```




```input2
?5?
4
2203
5229
276
6243
2 1 6 1 1 2 5 2 2 3

```




```output1
4

```




```output2
62

```



## Note

<p>In the second sample input, the optimal way is to compose the number <span class="tex-font-style-tt">453</span>. After adding this number, Boris will have numbers <span class="tex-font-style-tt">2656</span>, <span class="tex-font-style-tt">5682</span>, <span class="tex-font-style-tt">729</span> and <span class="tex-font-style-tt">6696</span>. The total cost of all digits in them is equal to <span class="tex-span">18 + 15 + 11 + 18 = 62</span>. </p>
