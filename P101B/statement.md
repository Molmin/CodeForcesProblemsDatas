## Description

<div><p>Little boy Gerald studies at school which is quite far from his house. That's why he has to go there by bus every day. The way from home to school is represented by a segment of a straight line; the segment contains exactly <span class="tex-span"><i>n</i> + 1</span> bus stops. All of them are numbered with integers from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i></span> in the order in which they follow from Gerald's home. The bus stop by Gerald's home has number <span class="tex-span">0</span> and the bus stop by the school has number <span class="tex-span"><i>n</i></span>.</p><p>There are <span class="tex-span"><i>m</i></span> buses running between the house and the school: the <span class="tex-span"><i>i</i></span>-th bus goes from stop <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> &lt; <i>t</i><sub class="lower-index"><i>i</i></sub></span>), visiting all the intermediate stops in the order in which they follow on the segment. Besides, Gerald's no idiot and he wouldn't get off the bus until it is still possible to ride on it closer to the school (obviously, getting off would be completely pointless). In other words, Gerald can get on the <span class="tex-span"><i>i</i></span>-th bus on any stop numbered from <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> - 1</span> inclusive, but he can get off the <span class="tex-span"><i>i</i></span>-th bus only on the bus stop <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Gerald can't walk between the bus stops and he also can't move in the direction from the school to the house.</p><p>Gerald wants to know how many ways he has to get from home to school. Tell him this number. Two ways are considered different if Gerald crosses some segment between the stops on different buses. As the number of ways can be too much, find the remainder of a division of this number by <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div><div class="input-specification"><p>The first line contains two space-separated integers: <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup>, 0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>). Then follow <span class="tex-span"><i>m</i></span> lines each containing two integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub></span>. They are the numbers of starting stops and end stops of the buses (<span class="tex-span">0 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> &lt; <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p></div><div class="output-specification"><p>Print the only number — the number of ways to get to the school modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div>

## Input

<p>The first line contains two space-separated integers: <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup>, 0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>). Then follow <span class="tex-span"><i>m</i></span> lines each containing two integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub></span>. They are the numbers of starting stops and end stops of the buses (<span class="tex-span">0 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> &lt; <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p>

## Output

<p>Print the only number — the number of ways to get to the school modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p>





```input1
2 2
0 1
1 2

```




```input2
3 2
0 1
1 2

```




```input3
5 5
0 1
0 2
0 3
0 4
0 5

```




```output1
1

```




```output2
0

```




```output3
16

```



## Note

<p>The first test has the only variant to get to school: first on bus number one to the bus stop number one; then on bus number two to the bus stop number two.</p><p>In the second test no bus goes to the third bus stop, where the school is positioned. Thus, the correct answer is <span class="tex-span">0</span>.</p><p>In the third test Gerald can either get or not on any of the first four buses to get closer to the school. Thus, the correct answer is <span class="tex-span">2<sup class="upper-index">4</sup> = 16</span>.</p>
