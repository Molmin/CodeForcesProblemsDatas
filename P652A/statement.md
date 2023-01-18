## Description

<div><p>The <span class="tex-span">9</span>-th grade student Gabriel noticed a caterpillar on a tree when walking around in a forest after the classes. The caterpillar was on the height <span class="tex-span"><i>h</i><sub class="lower-index">1</sub></span> cm from the ground. On the height <span class="tex-span"><i>h</i><sub class="lower-index">2</sub></span> cm (<span class="tex-span"><i>h</i><sub class="lower-index">2</sub> &gt; <i>h</i><sub class="lower-index">1</sub></span>) on the same tree hung an apple and the caterpillar was crawling to the apple.</p><p>Gabriel is interested when the caterpillar gets the apple. He noted that the caterpillar goes up by <span class="tex-span"><i>a</i></span> cm per hour by day and slips down by <span class="tex-span"><i>b</i></span> cm per hour by night.</p><p>In how many days Gabriel should return to the forest to see the caterpillar get the apple. You can consider that the day starts at <span class="tex-span">10</span> am and finishes at <span class="tex-span">10</span> pm. Gabriel's classes finish at <span class="tex-span">2</span> pm. You can consider that Gabriel noticed the caterpillar just after the classes at <span class="tex-span">2</span> pm.</p><p>Note that the forest is magic so the caterpillar can slip down under the ground and then lift to the apple.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>h</i><sub class="lower-index">1</sub>, <i>h</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index">1</sub> &lt; <i>h</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">5</sup></span>) — the heights of the position of the caterpillar and the apple in centimeters.</p><p>The second line contains two integers <span class="tex-span"><i>a</i>, <i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">5</sup></span>) — the distance the caterpillar goes up by day and slips down by night, in centimeters per hour.</p></div><div class="output-specification"><p>Print the only integer <span class="tex-span"><i>k</i></span> — the number of days Gabriel should wait to return to the forest and see the caterpillar getting the apple.</p><p>If the caterpillar can't get the apple print the only integer <span class="tex-span"> - 1</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>h</i><sub class="lower-index">1</sub>, <i>h</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index">1</sub> &lt; <i>h</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">5</sup></span>) — the heights of the position of the caterpillar and the apple in centimeters.</p><p>The second line contains two integers <span class="tex-span"><i>a</i>, <i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">5</sup></span>) — the distance the caterpillar goes up by day and slips down by night, in centimeters per hour.</p>

## Output

<p>Print the only integer <span class="tex-span"><i>k</i></span> — the number of days Gabriel should wait to return to the forest and see the caterpillar getting the apple.</p><p>If the caterpillar can't get the apple print the only integer <span class="tex-span"> - 1</span>.</p>





```input1
10 30
2 1

```




```input2
10 13
1 1

```




```input3
10 19
1 2

```




```input4
1 50
5 4

```




```output1
1

```




```output2
0

```




```output3
-1

```




```output4
1

```



## Note

<p>In the first example at <span class="tex-span">10</span> pm of the first day the caterpillar gets the height <span class="tex-span">26</span>. At <span class="tex-span">10</span> am of the next day it slips down to the height <span class="tex-span">14</span>. And finally at <span class="tex-span">6</span> pm of the same day the caterpillar gets the apple.</p><p>Note that in the last example the caterpillar was slipping down under the ground and getting the apple on the next day.</p>
