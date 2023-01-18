## Description

<div><p>Polycarp plans to conduct a load testing of its new project Fakebook. He already agreed with his friends that at certain points in time they will send requests to Fakebook. The load testing will last <span class="tex-span"><i>n</i></span> minutes and in the <span class="tex-span"><i>i</i></span>-th minute friends will send <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> requests.</p><p>Polycarp plans to test Fakebook under a special kind of load. In case the information about Fakebook gets into the mass media, Polycarp hopes for a monotone increase of the load, followed by a monotone decrease of the interest to the service. Polycarp wants to test this form of load.</p><p>Your task is to determine how many requests Polycarp must add so that before some moment the load on the server strictly increases and after that moment strictly decreases. Both the increasing part and the decreasing part can be empty (i. e. absent). The decrease should immediately follow the increase. In particular, the load with two equal neigbouring values is unacceptable.</p><p>For example, if the load is described with one of the arrays <span class="tex-font-style-tt">[1, 2, 8, 4, 3]</span>, <span class="tex-font-style-tt">[1, 3, 5]</span> or <span class="tex-font-style-tt">[10]</span>, then such load satisfies Polycarp (in each of the cases there is an increasing part, immediately followed with a decreasing part). If the load is described with one of the arrays <span class="tex-font-style-tt">[1, 2, 2, 1]</span>, <span class="tex-font-style-tt">[2, 1, 2]</span> or <span class="tex-font-style-tt">[10, 10]</span>, then such load does not satisfy Polycarp.</p><p>Help Polycarp to make the minimum number of additional requests, so that the resulting load satisfies Polycarp. He can make any number of additional requests at any minute from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>) — the duration of the load testing.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of requests from friends in the <span class="tex-span"><i>i</i></span>-th minute of the load testing.</p></div><div class="output-specification"><p>Print the minimum number of additional requests from Polycarp that would make the load strictly increasing in the beginning and then strictly decreasing afterwards.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>) — the duration of the load testing.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of requests from friends in the <span class="tex-span"><i>i</i></span>-th minute of the load testing.</p>

## Output

<p>Print the minimum number of additional requests from Polycarp that would make the load strictly increasing in the beginning and then strictly decreasing afterwards.</p>





```input1
5
1 4 3 2 5

```




```input2
5
1 2 2 2 1

```




```input3
7
10 20 40 50 70 90 30

```




```output1
6

```




```output2
1

```




```output3
0

```



## Note

<p>In the first example Polycarp must make two additional requests in the third minute and four additional requests in the fourth minute. So the resulting load will look like: <span class="tex-font-style-tt">[1, 4, 5, 6, 5]</span>. In total, Polycarp will make <span class="tex-span">6</span> additional requests.</p><p>In the second example it is enough to make one additional request in the third minute, so the answer is <span class="tex-span">1</span>.</p><p>In the third example the load already satisfies all conditions described in the statement, so the answer is <span class="tex-span">0</span>.</p>
