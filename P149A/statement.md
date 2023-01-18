## Description

<div><p>What joy! Petya's parents went on a business trip for the whole year and the playful kid is left all by himself. Petya got absolutely happy. He jumped on the bed and threw pillows all day long, until... </p><p>Today Petya opened the cupboard and found a scary note there. His parents had left him with duties: he should water their favourite flower all year, each day, in the morning, in the afternoon and in the evening. "Wait a second!" — thought Petya. He know for a fact that if he fulfills the parents' task in the <span class="tex-span"><i>i</i></span>-th (<span class="tex-span">1 ≤ <i>i</i> ≤ 12</span>) month of the year, then the flower will grow by <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> centimeters, and if he doesn't water the flower in the <span class="tex-span"><i>i</i></span>-th month, then the flower won't grow this month. Petya also knows that try as he might, his parents won't believe that he has been watering the flower if it grows strictly less than by <span class="tex-span"><i>k</i></span> centimeters. </p><p>Help Petya choose the minimum number of months when he will water the flower, given that the flower should grow no less than by <span class="tex-span"><i>k</i></span> centimeters.</p></div><div class="input-specification"><p>The first line contains exactly one integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 100</span>). The next line contains twelve space-separated integers: the <span class="tex-span"><i>i</i></span>-th (<span class="tex-span">1 ≤ <i>i</i> ≤ 12</span>) number in the line represents <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>). </p></div><div class="output-specification"><p>Print the only integer — the minimum number of months when Petya has to water the flower so that the flower grows no less than by <span class="tex-span"><i>k</i></span> centimeters. If the flower can't grow by <span class="tex-span"><i>k</i></span> centimeters in a year, print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains exactly one integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 100</span>). The next line contains twelve space-separated integers: the <span class="tex-span"><i>i</i></span>-th (<span class="tex-span">1 ≤ <i>i</i> ≤ 12</span>) number in the line represents <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>). </p>

## Output

<p>Print the only integer — the minimum number of months when Petya has to water the flower so that the flower grows no less than by <span class="tex-span"><i>k</i></span> centimeters. If the flower can't grow by <span class="tex-span"><i>k</i></span> centimeters in a year, print <span class="tex-font-style-tt">-1</span>.</p>





```input1
5
1 1 1 1 2 2 3 2 2 1 1 1

```




```input2
0
0 0 0 0 0 0 0 1 1 2 3 0

```




```input3
11
1 1 4 1 1 5 1 1 4 1 1 1

```




```output1
2

```




```output2
0

```




```output3
3

```



## Note

<p>Let's consider the first sample test. There it is enough to water the flower during the seventh and the ninth month. Then the flower grows by exactly five centimeters.</p><p>In the second sample Petya's parents will believe him even if the flower doesn't grow at all (<span class="tex-span"><i>k</i> = 0</span>). So, it is possible for Petya not to water the flower at all.</p>
