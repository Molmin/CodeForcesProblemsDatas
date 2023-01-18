## Description

<div><p>Zxr960115 is owner of a large farm. He feeds <span class="tex-span"><i>m</i></span> cute cats and employs <span class="tex-span"><i>p</i></span> feeders. There's a straight road across the farm and <span class="tex-span"><i>n</i></span> hills along the road, numbered from 1 to <span class="tex-span"><i>n</i></span> from left to right. The distance between hill <span class="tex-span"><i>i</i></span> and <span class="tex-span">(<i>i</i> - 1)</span> is <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> meters. The feeders live in hill 1.</p><p>One day, the cats went out to play. Cat <span class="tex-span"><i>i</i></span> went on a trip to hill <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>, finished its trip at time <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, and then waited at hill <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> for a feeder. The feeders must take all the cats. Each feeder goes straightly from hill 1 to <span class="tex-span"><i>n</i></span> without waiting at a hill and takes all the <span class="tex-font-style-bf">waiting</span> cats at each hill away. Feeders walk at a speed of 1 meter per unit time and are strong enough to take as many cats as they want.</p><p>For example, suppose we have two hills <span class="tex-span">(<i>d</i><sub class="lower-index">2</sub> = 1)</span> and one cat that finished its trip at time 3 at hill 2 <span class="tex-span">(<i>h</i><sub class="lower-index">1</sub> = 2)</span>. Then if the feeder leaves hill 1 at time 2 or at time 3, he can take this cat, but if he leaves hill 1 at time 1 he can't take it. If the feeder leaves hill 1 at time 2, the cat waits him for 0 time units, if the feeder leaves hill 1 at time 3, the cat waits him for 1 time units.</p><p>Your task is to schedule the time leaving from hill 1 for each feeder so that the sum of the waiting time of all cats is minimized.</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>p</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>p</i> ≤ 100)</span>.</p><p>The second line contains <span class="tex-span"><i>n</i> - 1</span> positive integers <span class="tex-span"><i>d</i><sub class="lower-index">2</sub>, <i>d</i><sub class="lower-index">3</sub>, ..., <i>d</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> &lt; 10<sup class="upper-index">4</sup>)</span>.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p></div><div class="output-specification"><p>Output an integer, the minimum sum of waiting time of all cats.</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>p</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>p</i> ≤ 100)</span>.</p><p>The second line contains <span class="tex-span"><i>n</i> - 1</span> positive integers <span class="tex-span"><i>d</i><sub class="lower-index">2</sub>, <i>d</i><sub class="lower-index">3</sub>, ..., <i>d</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> &lt; 10<sup class="upper-index">4</sup>)</span>.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p>

## Output

<p>Output an integer, the minimum sum of waiting time of all cats.</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
4 6 2
1 3 5
1 0
2 1
4 9
1 10
2 10
3 12

```




```output1
3

```


