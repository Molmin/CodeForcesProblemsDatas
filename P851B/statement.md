## Description

<div><p>Arpa is taking a geometry exam. Here is the last problem of the exam.</p><p>You are given three points <span class="tex-span"><i>a</i>, <i>b</i>, <i>c</i></span>.</p><p>Find a point and an angle such that if we rotate the page around the point by the angle, the new position of <span class="tex-span"><i>a</i></span> is the same as the old position of <span class="tex-span"><i>b</i></span>, and the new position of <span class="tex-span"><i>b</i></span> is the same as the old position of <span class="tex-span"><i>c</i></span>.</p><p>Arpa is doubting if the problem has a solution or not (i.e. if there exists a point and an angle satisfying the condition). Help Arpa determine if the question has a solution or not.</p></div><div class="input-specification"><p>The only line contains six integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>x</i></sub>, <i>a</i><sub class="lower-index"><i>y</i></sub>, <i>b</i><sub class="lower-index"><i>x</i></sub>, <i>b</i><sub class="lower-index"><i>y</i></sub>, <i>c</i><sub class="lower-index"><i>x</i></sub>, <i>c</i><sub class="lower-index"><i>y</i></sub></span> (<span class="tex-span">|<i>a</i><sub class="lower-index"><i>x</i></sub>|, |<i>a</i><sub class="lower-index"><i>y</i></sub>|, |<i>b</i><sub class="lower-index"><i>x</i></sub>|, |<i>b</i><sub class="lower-index"><i>y</i></sub>|, |<i>c</i><sub class="lower-index"><i>x</i></sub>|, |<i>c</i><sub class="lower-index"><i>y</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>). It's guaranteed that the points are distinct.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">Yes</span>" if the problem has a solution, "<span class="tex-font-style-tt">No</span>" otherwise.</p><p>You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The only line contains six integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>x</i></sub>, <i>a</i><sub class="lower-index"><i>y</i></sub>, <i>b</i><sub class="lower-index"><i>x</i></sub>, <i>b</i><sub class="lower-index"><i>y</i></sub>, <i>c</i><sub class="lower-index"><i>x</i></sub>, <i>c</i><sub class="lower-index"><i>y</i></sub></span> (<span class="tex-span">|<i>a</i><sub class="lower-index"><i>x</i></sub>|, |<i>a</i><sub class="lower-index"><i>y</i></sub>|, |<i>b</i><sub class="lower-index"><i>x</i></sub>|, |<i>b</i><sub class="lower-index"><i>y</i></sub>|, |<i>c</i><sub class="lower-index"><i>x</i></sub>|, |<i>c</i><sub class="lower-index"><i>y</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>). It's guaranteed that the points are distinct.</p>

## Output

<p>Print "<span class="tex-font-style-tt">Yes</span>" if the problem has a solution, "<span class="tex-font-style-tt">No</span>" otherwise.</p><p>You can print each letter in any case (upper or lower).</p>





```input1
0 1 1 1 1 0

```




```input2
1 1 0 0 1000 1000

```




```output1
Yes

```




```output2
No

```



## Note

<p>In the first sample test, rotate the page around <span class="tex-span">(0.5, 0.5)</span> by <img align="middle" class="tex-formula" src="file://dM3CxeG3.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>In the second sample test, you can't find any solution.</p>
