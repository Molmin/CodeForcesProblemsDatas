## Description

<div><p>The main Bertown street is represented by a straight line. There are <span class="tex-span">10<sup class="upper-index">9</sup></span> bus stops located on the line. The stops are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span">10<sup class="upper-index">9</sup></span> in the order in which they follow on the road. The city has <span class="tex-span"><i>n</i></span> buses. Every day the <span class="tex-span"><i>i</i></span>-th bus drives from stop number <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> to stop number <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> &lt; <i>f</i><sub class="lower-index"><i>i</i></sub></span>), it stops on all intermediate stops and returns only at night. The bus starts driving at time <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and drives so fast that it finishes driving also at time <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>. The time <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is different for all buses. The buses have infinite capacity.</p><p>Bertown has <span class="tex-span"><i>m</i></span> citizens. Today the <span class="tex-span"><i>i</i></span>-th person should get from stop number <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> to stop number <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub></span>); the <span class="tex-span"><i>i</i></span>-th citizen comes to his initial stop (<span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>) at time <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. Each person, on the one hand, wants to get to the destination point as quickly as possible, and on the other hand, definitely does not want to change the buses as he rides. More formally: the <span class="tex-span"><i>i</i></span>-th person chooses bus <span class="tex-span"><i>j</i></span>, with minimum time <span class="tex-span"><i>t</i><sub class="lower-index"><i>j</i></sub></span>, such that <span class="tex-span"><i>s</i><sub class="lower-index"><i>j</i></sub> ≤ <i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>f</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>t</i><sub class="lower-index"><i>j</i></sub></span>. </p><p>Your task is to determine for each citizen whether he can ride to the destination point today and if he can, find the number of the bus on which the citizen will ride.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of buses and the number of people. </p><p>Then <span class="tex-span"><i>n</i></span> lines follow, each of them contains three integers: <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub>, <i>f</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>, <i>s</i><sub class="lower-index"><i>i</i></sub> &lt; <i>f</i><sub class="lower-index"><i>i</i></sub></span>) — the description of the buses. It is guaranteed that all <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>-s are different.</p><p>Then <span class="tex-span"><i>m</i></span> lines follow, each of them contains three integers: <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>, <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub></span>) — the Bertown citizens' description. Some <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>-s could coincide.</p></div><div class="output-specification"><p>In the first line print <span class="tex-span"><i>m</i></span> space-separated integers: the <span class="tex-span"><i>i</i></span>-th number should be equal either to -1, if the person number <span class="tex-span"><i>i</i></span> can't get to the destination point, or to the number of the bus that will ride the person number <span class="tex-span"><i>i</i></span>. The buses are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in the input order.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of buses and the number of people. </p><p>Then <span class="tex-span"><i>n</i></span> lines follow, each of them contains three integers: <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub>, <i>f</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>, <i>s</i><sub class="lower-index"><i>i</i></sub> &lt; <i>f</i><sub class="lower-index"><i>i</i></sub></span>) — the description of the buses. It is guaranteed that all <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>-s are different.</p><p>Then <span class="tex-span"><i>m</i></span> lines follow, each of them contains three integers: <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>, <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub></span>) — the Bertown citizens' description. Some <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>-s could coincide.</p>

## Output

<p>In the first line print <span class="tex-span"><i>m</i></span> space-separated integers: the <span class="tex-span"><i>i</i></span>-th number should be equal either to -1, if the person number <span class="tex-span"><i>i</i></span> can't get to the destination point, or to the number of the bus that will ride the person number <span class="tex-span"><i>i</i></span>. The buses are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in the input order.</p>





```input1
4 3
1 10 10
5 6 2
6 7 3
5 7 4
5 7 1
1 2 1
1 10 11

```




```input2
1 1
1 1000000000 1000000000
1 1000000000 1000000000

```




```output1
4 1 -1

```




```output2
1

```


