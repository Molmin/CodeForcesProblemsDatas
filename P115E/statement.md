## Description

<div><p>You are a car race organizer and would like to arrange some races in Linear Kingdom.</p><p>Linear Kingdom has <span class="tex-span"><i>n</i></span> consecutive roads spanning from left to right. The roads are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from left to right, thus the roads follow in the order of their numbers' increasing. There will be several races that may be held on these roads. Each race will use a <span class="tex-font-style-bf">consecutive</span> subset of these roads. Also, each race will pay some amount of money to you if this race is held. No races overlap in time, so some roads can be used in several races.</p><p>Unfortunately, some of the roads are in a bad condition and they need repair. Each road has repair costs associated with it, you are required to pay this cost to repair the road. A race can only take place if all the roads used in the race are renovated. Your task is to repair such roads (possibly all or none) that will maximize your profit. Your profit is defined as the total money you get from the races that are held minus the total money you spent to repair the roads. Note that you may decide not to repair any road and gain zero profit.</p><p>Print the maximum profit you can gain.</p></div><div class="input-specification"><p>The first line contains two single-space separated integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>), denoting the number of roads and the number of races, respectively.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow, each line will contain a single non-negative integer not exceeding <span class="tex-span">10<sup class="upper-index">9</sup></span> denoting the cost to repair a road. The costs are given in order from road <span class="tex-span">1</span> to road <span class="tex-span"><i>n</i></span>.</p><p>Finally, <span class="tex-span"><i>m</i></span> lines follow. Each line is single-space-separated triplets of integers. Each triplet will be given as <span class="tex-span"><i>lb</i></span>, <span class="tex-span"><i>ub</i></span>, and <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>lb</i> ≤ <i>ub</i> ≤ <i>n</i>, 1 ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup></span>), which means that the race these three integers describe will use all the roads from <span class="tex-span"><i>lb</i></span> to <span class="tex-span"><i>ub</i></span>, inclusive, and if it's held you get <span class="tex-span"><i>p</i></span>.</p></div><div class="output-specification"><p>Print a single integer denoting the maximum possible profit you can gain.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is recommended to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> stream (also you may use <span class="tex-font-style-tt">%I64d</span> specificator).</p></div>

## Input

<p>The first line contains two single-space separated integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>), denoting the number of roads and the number of races, respectively.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow, each line will contain a single non-negative integer not exceeding <span class="tex-span">10<sup class="upper-index">9</sup></span> denoting the cost to repair a road. The costs are given in order from road <span class="tex-span">1</span> to road <span class="tex-span"><i>n</i></span>.</p><p>Finally, <span class="tex-span"><i>m</i></span> lines follow. Each line is single-space-separated triplets of integers. Each triplet will be given as <span class="tex-span"><i>lb</i></span>, <span class="tex-span"><i>ub</i></span>, and <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>lb</i> ≤ <i>ub</i> ≤ <i>n</i>, 1 ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup></span>), which means that the race these three integers describe will use all the roads from <span class="tex-span"><i>lb</i></span> to <span class="tex-span"><i>ub</i></span>, inclusive, and if it's held you get <span class="tex-span"><i>p</i></span>.</p>

## Output

<p>Print a single integer denoting the maximum possible profit you can gain.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is recommended to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> stream (also you may use <span class="tex-font-style-tt">%I64d</span> specificator).</p>





```input1
7 4
3
2
3
2
1
2
3
1 2 5
2 3 5
3 5 3
7 7 5

```




```input2
2 1
0
3
1 2 5

```




```input3
3 1
10
10
10
1 3 10

```




```output1
4

```




```output2
2

```




```output3
0

```



## Note

<p>In the first sample the optimal solution is to repair roads <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">3</span>, and <span class="tex-span">7</span>. Three races will take place which nets you <span class="tex-span">15</span>. The road repair costs <span class="tex-span">11</span>, hence your profit is <span class="tex-span">4</span>.</p>
