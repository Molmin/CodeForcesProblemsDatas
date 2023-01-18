## Description

<div><p>There are <span class="tex-span"><i>n</i></span> cities and <span class="tex-span"><i>n</i> - 1</span> roads in the Seven Kingdoms, each road connects two cities and we can reach any city from any other by the roads.</p><p>Theon and Yara Greyjoy are on a horse in the first city, they are starting traveling through the roads. But the weather is foggy, so they can’t see where the horse brings them. When the horse reaches a city (including the first one), it goes to one of the cities connected to the current city. But it is a strange horse, it only goes to cities in which they weren't before. In each such city, the horse goes with equal probabilities and it stops when there are no such cities. </p><p>Let the length of each road be <span class="tex-span">1</span>. The journey starts in the city <span class="tex-span">1</span>. What is the expected length (expected value of length) of their journey? You can read about expected (average) value by the link <a href="https://en.wikipedia.org/wiki/Expected_value">https://en.wikipedia.org/wiki/Expected_value</a>.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100000</span>)&nbsp;— number of cities.</p><p>Then <span class="tex-span"><i>n</i> - 1</span> lines follow. The <span class="tex-span"><i>i</i></span>-th line of these lines contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— the cities connected by the <span class="tex-span"><i>i</i></span>-th road.</p><p>It is guaranteed that one can reach any city from any other by the roads.</p></div><div class="output-specification"><p>Print a number&nbsp;— the expected length of their journey. The journey starts in the city <span class="tex-span">1</span>.</p><p>Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://gPEvaIRx.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100000</span>)&nbsp;— number of cities.</p><p>Then <span class="tex-span"><i>n</i> - 1</span> lines follow. The <span class="tex-span"><i>i</i></span>-th line of these lines contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— the cities connected by the <span class="tex-span"><i>i</i></span>-th road.</p><p>It is guaranteed that one can reach any city from any other by the roads.</p>

## Output

<p>Print a number&nbsp;— the expected length of their journey. The journey starts in the city <span class="tex-span">1</span>.</p><p>Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://gPEvaIRx.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
4
1 2
1 3
2 4

```




```input2
5
1 2
1 3
3 4
2 5

```




```output1
1.500000000000000

```




```output2
2.000000000000000

```



## Note

<p>In the first sample, their journey may end in cities <span class="tex-span">3</span> or <span class="tex-span">4</span> with equal probability. The distance to city <span class="tex-span">3</span> is <span class="tex-span">1</span> and to city <span class="tex-span">4</span> is <span class="tex-span">2</span>, so the expected length is <span class="tex-span">1.5</span>.</p><p>In the second sample, their journey may end in city <span class="tex-span">4</span> or <span class="tex-span">5</span>. The distance to the both cities is <span class="tex-span">2</span>, so the expected length is <span class="tex-span">2</span>.</p>
