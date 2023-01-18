## Description

<div><p>On vacations <span class="tex-span"><i>n</i></span> pupils decided to go on excursion and gather all together. They need to overcome the path with the length <span class="tex-span"><i>l</i></span> meters. Each of the pupils will go with the speed equal to <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span>. To get to the excursion quickly, it was decided to rent a bus, which has seats for <span class="tex-span"><i>k</i></span> people (it means that it can't fit more than <span class="tex-span"><i>k</i></span> people at the same time) and the speed equal to <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span>. In order to avoid seasick, each of the pupils want to get into the bus <span class="tex-font-style-bf">no more than once</span>.</p><p>Determine the minimum time required for all <span class="tex-span"><i>n</i></span> pupils to reach the place of excursion. Consider that the embarkation and disembarkation of passengers, as well as the reversal of the bus, take place immediately and this time can be neglected. </p></div><div class="input-specification"><p>The first line of the input contains five positive integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10 000</span>, <span class="tex-span">1 ≤ <i>l</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>v</i><sub class="lower-index">1</sub> &lt; <i>v</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>)&nbsp;— the number of pupils, the distance from meeting to the place of excursion, the speed of each pupil, the speed of bus and the number of seats in the bus. </p></div><div class="output-specification"><p>Print the real number&nbsp;— the minimum time in which all pupils can reach the place of excursion. Your answer will be considered correct if its absolute or relative error won't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line of the input contains five positive integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10 000</span>, <span class="tex-span">1 ≤ <i>l</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>v</i><sub class="lower-index">1</sub> &lt; <i>v</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>)&nbsp;— the number of pupils, the distance from meeting to the place of excursion, the speed of each pupil, the speed of bus and the number of seats in the bus. </p>

## Output

<p>Print the real number&nbsp;— the minimum time in which all pupils can reach the place of excursion. Your answer will be considered correct if its absolute or relative error won't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
5 10 1 2 5

```




```input2
3 6 1 2 1

```




```output1
5.0000000000

```




```output2
4.7142857143

```



## Note

<p>In the first sample we should immediately put all five pupils to the bus. The speed of the bus equals <span class="tex-span">2</span> and the distance is equal to <span class="tex-span">10</span>, so the pupils will reach the place of excursion in time <span class="tex-span">10 / 2 = 5</span>.</p>
