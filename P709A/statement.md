## Description

<div><p>Kolya is going to make fresh orange juice. He has <span class="tex-span"><i>n</i></span> oranges of sizes <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. Kolya will put them in the juicer in the fixed order, starting with orange of size <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, then orange of size <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> and so on. To be put in the juicer the orange must have size not exceeding <span class="tex-span"><i>b</i></span>, so if Kolya sees an orange that is strictly greater he throws it away and continues with the next one.</p><p>The juicer has a special section to collect waste. It overflows if Kolya squeezes oranges of the total size strictly greater than <span class="tex-span"><i>d</i></span>. When it happens Kolya empties the waste section (even if there are no more oranges) and continues to squeeze the juice. How many times will he have to empty the waste section?</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>b</i> ≤ <i>d</i> ≤ 1 000 000</span>)&nbsp;— the number of oranges, the maximum size of the orange that fits in the juicer and the value <span class="tex-span"><i>d</i></span>, which determines the condition when the waste section should be emptied.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>)&nbsp;— sizes of the oranges listed in the order Kolya is going to try to put them in the juicer.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the number of times Kolya will have to empty the waste section.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>b</i> ≤ <i>d</i> ≤ 1 000 000</span>)&nbsp;— the number of oranges, the maximum size of the orange that fits in the juicer and the value <span class="tex-span"><i>d</i></span>, which determines the condition when the waste section should be emptied.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>)&nbsp;— sizes of the oranges listed in the order Kolya is going to try to put them in the juicer.</p>

## Output

<p>Print one integer&nbsp;— the number of times Kolya will have to empty the waste section.</p>





```input1
2 7 10
5 6

```




```input2
1 5 10
7

```




```input3
3 10 10
5 7 7

```




```input4
1 1 1
1

```




```output1
1

```




```output2
0

```




```output3
1

```




```output4
0

```



## Note

<p>In the first sample, Kolya will squeeze the juice from two oranges and empty the waste section afterwards.</p><p>In the second sample, the orange won't fit in the juicer so Kolya will have no juice at all.</p>
