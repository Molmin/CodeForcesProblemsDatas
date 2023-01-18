## Description

<div><p>Duff is addicted to meat! Malek wants to keep her happy for <span class="tex-span"><i>n</i></span> days. In order to be happy in <span class="tex-span"><i>i</i></span>-th day, she needs to eat exactly <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> kilograms of meat.</p><center> <img class="tex-graphics" src="file://x9oie6DN.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>There is a big shop uptown and Malek wants to buy meat for her from there. In <span class="tex-span"><i>i</i></span>-th day, they sell meat for <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> dollars per kilogram. Malek knows all numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> and <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span>. In each day, he can buy arbitrary amount of meat, also he can keep some meat he has for the future.</p><p>Malek is a little tired from cooking meat, so he asked for your help. Help him to minimize the total money he spends to keep Duff happy for <span class="tex-span"><i>n</i></span> days. </p></div><div class="input-specification"><p>The first line of input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of days.</p><p>In the next <span class="tex-span"><i>n</i></span> lines, <span class="tex-span"><i>i</i></span>-th line contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), the amount of meat Duff needs and the cost of meat in that day.</p></div><div class="output-specification"><p>Print the minimum money needed to keep Duff happy for <span class="tex-span"><i>n</i></span> days, in one line.</p></div>

## Input

<p>The first line of input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of days.</p><p>In the next <span class="tex-span"><i>n</i></span> lines, <span class="tex-span"><i>i</i></span>-th line contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), the amount of meat Duff needs and the cost of meat in that day.</p>

## Output

<p>Print the minimum money needed to keep Duff happy for <span class="tex-span"><i>n</i></span> days, in one line.</p>





```input1
3
1 3
2 2
3 1

```




```input2
3
1 3
2 1
3 2

```




```output1
10

```




```output2
8

```



## Note

<p>In the first sample case: An optimal way would be to buy 1 kg on the first day, 2 kg on the second day and 3 kg on the third day.</p><p>In the second sample case: An optimal way would be to buy 1 kg on the first day and 5 kg (needed meat for the second and third day) on the second day.</p>
