## Description

<div><p>Luba thinks about watering her garden. The garden can be represented as a segment of length <span class="tex-span"><i>k</i></span>. Luba has got <span class="tex-span"><i>n</i></span> buckets, the <span class="tex-span"><i>i</i></span>-th bucket allows her to water some continuous subsegment of garden of length <span class="tex-font-style-bf">exactly</span> <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> each hour. <span class="tex-font-style-bf">Luba can't water any parts of the garden that were already watered, also she can't water the ground outside the garden</span>.</p><p>Luba has to choose <span class="tex-font-style-bf">one</span> of the buckets in order to water the garden as fast as possible (as mentioned above, each hour she will water some continuous subsegment of length <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> if she chooses the <span class="tex-span"><i>i</i></span>-th bucket). Help her to determine the minimum number of hours she has to spend watering the garden. It is guaranteed that Luba can always choose a bucket so it is possible water the garden.</p><p>See the examples for better understanding.</p></div><div class="input-specification"><p>The first line of input contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 100</span>) — the number of buckets and the length of the garden, respectively.</p><p>The second line of input contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the length of the segment that can be watered by the <span class="tex-span"><i>i</i></span>-th bucket in one hour.</p><p>It is guaranteed that there is at least one bucket such that it is possible to water the garden in integer number of hours using only this bucket.</p></div><div class="output-specification"><p>Print one integer number — the minimum number of hours required to water the garden.</p></div>

## Input

<p>The first line of input contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 100</span>) — the number of buckets and the length of the garden, respectively.</p><p>The second line of input contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the length of the segment that can be watered by the <span class="tex-span"><i>i</i></span>-th bucket in one hour.</p><p>It is guaranteed that there is at least one bucket such that it is possible to water the garden in integer number of hours using only this bucket.</p>

## Output

<p>Print one integer number — the minimum number of hours required to water the garden.</p>





```input1
3 6
2 3 5

```




```input2
6 7
1 2 3 4 5 6

```




```output1
2

```




```output2
7

```



## Note

<p>In the first test the best option is to choose the bucket that allows to water the segment of length <span class="tex-span">3</span>. We can't choose the bucket that allows to water the segment of length <span class="tex-span">5</span> because then we can't water the whole garden.</p><p>In the second test we can choose only the bucket that allows us to water the segment of length <span class="tex-span">1</span>.</p>
