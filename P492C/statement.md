## Description

<div><p>Vanya wants to pass <span class="tex-span"><i>n</i></span> exams and get the academic scholarship. He will get the scholarship if the average grade mark for all the exams is at least <span class="tex-span"><i>avg</i></span>. The exam grade cannot exceed <span class="tex-span"><i>r</i></span>. Vanya has passed the exams and got grade <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> for the <span class="tex-span"><i>i</i></span>-th exam. To increase the grade for the <span class="tex-span"><i>i</i></span>-th exam by 1 point, Vanya must write <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> essays. He can raise the exam grade multiple times.</p><p>What is the minimum number of essays that Vanya needs to write to get scholarship?</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>avg</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>r</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>avg</i> ≤ <i>min</i>(<i>r</i>, 10<sup class="upper-index">6</sup>)</span>)&nbsp;— the number of exams, the maximum grade and the required grade point average, respectively.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i></span>, <span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>).</p></div><div class="output-specification"><p>In the first line print the minimum number of essays.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>avg</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>r</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>avg</i> ≤ <i>min</i>(<i>r</i>, 10<sup class="upper-index">6</sup>)</span>)&nbsp;— the number of exams, the maximum grade and the required grade point average, respectively.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i></span>, <span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>).</p>

## Output

<p>In the first line print the minimum number of essays.</p>





```input1
5 5 4
5 2
4 7
3 1
3 2
2 5

```




```input2
2 5 4
5 2
5 2

```




```output1
4

```




```output2
0

```



## Note

<p>In the first sample Vanya can write 2 essays for the 3rd exam to raise his grade by 2 points and 2 essays for the 4th exam to raise his grade by 1 point.</p><p>In the second sample, Vanya doesn't need to write any essays as his general point average already is above average.</p>
