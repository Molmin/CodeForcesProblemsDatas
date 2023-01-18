## Description

<div><p>Princess Heidi decided to give orders to all her <span class="tex-span"><i>K</i></span> Rebel ship commanders in person. Unfortunately, she is currently travelling through hyperspace, and will leave it only at <span class="tex-span"><i>N</i></span> specific moments <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>N</i></sub></span>. The meetings with commanders must therefore start and stop at those times. Namely, each commander will board her ship at some time <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and disembark at some later time <span class="tex-span"><i>t</i><sub class="lower-index"><i>j</i></sub></span>. Of course, Heidi needs to meet with all commanders, and no two meetings can be held during the same time. Two commanders cannot even meet at the beginnings/endings of the hyperspace jumps, because too many ships in one position could give out their coordinates to the enemy. </p><p>Your task is to find minimum time that Princess Heidi has to spend on meetings, with her schedule satisfying the conditions above. </p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>K</i></span>, <span class="tex-span"><i>N</i></span> (<span class="tex-span">2 ≤ 2<i>K</i> ≤ <i>N</i> ≤ 500000</span>, <span class="tex-span"><i>K</i> ≤ 5000</span>). The second line contains <span class="tex-span"><i>N</i></span> distinct integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>N</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) representing the times when Heidi leaves hyperspace.</p></div><div class="output-specification"><p>Output only one integer: the minimum time spent on meetings. </p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>K</i></span>, <span class="tex-span"><i>N</i></span> (<span class="tex-span">2 ≤ 2<i>K</i> ≤ <i>N</i> ≤ 500000</span>, <span class="tex-span"><i>K</i> ≤ 5000</span>). The second line contains <span class="tex-span"><i>N</i></span> distinct integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>N</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) representing the times when Heidi leaves hyperspace.</p>

## Output

<p>Output only one integer: the minimum time spent on meetings. </p>





```input1
2 5
1 4 6 7 12

```




```input2
3 6
6 3 4 2 5 1

```




```input3
4 12
15 7 4 19 3 30 14 1 5 23 17 25

```




```output1
4

```




```output2
3

```




```output3
6

```



## Note

<p>In the first example, there are five valid schedules: <span class="tex-span">[1, 4], [6, 7]</span> with total time 4, <span class="tex-span">[1, 4], [6, 12]</span> with total time 9, <span class="tex-span">[1, 4], [7, 12]</span> with total time 8, <span class="tex-span">[1, 6], [7, 12]</span> with total time 10, and <span class="tex-span">[4, 6], [7, 12]</span> with total time 7. So the answer is 4.</p><p>In the second example, there is only 1 valid schedule: <span class="tex-span">[1, 2], [3, 4], [5, 6]</span>.</p><p>For the third example, one possible schedule with total time 6 is: <span class="tex-span">[1, 3], [4, 5], [14, 15], [23, 25]</span>.</p>
