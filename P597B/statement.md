## Description

<div><p>A restaurant received <span class="tex-span"><i>n</i></span> orders for the rental. Each rental order reserve the restaurant for a continuous period of time, the <span class="tex-span"><i>i</i></span>-th order is characterized by two time values — the start time <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and the finish time <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub></span>).</p><p>Restaurant management can accept and reject orders. What is the maximal number of orders the restaurant can accept?</p><p>No two accepted orders can intersect, i.e. they can't share even a moment of time. If one order ends in the moment other starts, they can't be accepted both.</p></div><div class="input-specification"><p>The first line contains integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>) — number of orders. The following <span class="tex-span"><i>n</i></span> lines contain integer values <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> each (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print the maximal number of orders that can be accepted.</p></div>

## Input

<p>The first line contains integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>) — number of orders. The following <span class="tex-span"><i>n</i></span> lines contain integer values <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> each (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print the maximal number of orders that can be accepted.</p>





```input1
2
7 11
4 7

```




```input2
5
1 2
2 3
3 4
4 5
5 6

```




```input3
6
4 8
1 5
4 7
2 5
1 3
6 8

```




```output1
1

```




```output2
3

```




```output3
2

```


