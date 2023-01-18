## Description

<div><p>Vasiliy spent his vacation in a sanatorium, came back and found that he completely forgot details of his vacation! </p><p>Every day there was a breakfast, a dinner and a supper in a dining room of the sanatorium (of course, in this order). The only thing that Vasiliy has now is a card from the dining room contaning notes how many times he had a breakfast, a dinner and a supper (thus, the card contains three integers). Vasiliy could sometimes have missed some meal, for example, he could have had a breakfast and a supper, but a dinner, or, probably, at some days he haven't been at the dining room at all.</p><p>Vasiliy doesn't remember what was the time of the day when he arrived to sanatorium (before breakfast, before dinner, before supper or after supper), and the time when he left it (before breakfast, before dinner, before supper or after supper). So he considers any of these options. After Vasiliy arrived to the sanatorium, he was there all the time until he left. Please note, that it's possible that Vasiliy left the sanatorium on the same day he arrived.</p><p>According to the notes in the card, help Vasiliy determine the minimum number of meals in the dining room that he could have missed. We shouldn't count as missed meals on the arrival day before Vasiliy's arrival and meals on the departure day after he left.</p></div><div class="input-specification"><p>The only line contains three integers <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>d</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">0 ≤ <i>b</i>, <i>d</i>, <i>s</i> ≤ 10<sup class="upper-index">18</sup>,  <i>b</i> + <i>d</i> + <i>s</i> ≥ 1</span>)&nbsp;— the number of breakfasts, dinners and suppers which Vasiliy had during his vacation in the sanatorium. </p></div><div class="output-specification"><p>Print single integer&nbsp;— the minimum possible number of meals which Vasiliy could have missed during his vacation. </p></div>

## Input

<p>The only line contains three integers <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>d</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">0 ≤ <i>b</i>, <i>d</i>, <i>s</i> ≤ 10<sup class="upper-index">18</sup>,  <i>b</i> + <i>d</i> + <i>s</i> ≥ 1</span>)&nbsp;— the number of breakfasts, dinners and suppers which Vasiliy had during his vacation in the sanatorium. </p>

## Output

<p>Print single integer&nbsp;— the minimum possible number of meals which Vasiliy could have missed during his vacation. </p>





```input1
3 2 1

```




```input2
1 0 0

```




```input3
1 1 1

```




```input4
1000000000000000000 0 1000000000000000000

```




```output1
1

```




```output2
0

```




```output3
0

```




```output4
999999999999999999

```



## Note

<p>In the first sample, Vasiliy could have missed one supper, for example, in case he have arrived before breakfast, have been in the sanatorium for two days (including the day of arrival) and then have left after breakfast on the third day. </p><p>In the second sample, Vasiliy could have arrived before breakfast, have had it, and immediately have left the sanatorium, not missing any meal.</p><p>In the third sample, Vasiliy could have been in the sanatorium for one day, not missing any meal. </p>
