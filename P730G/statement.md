## Description

<div><p>Polycarp starts his own business. Tomorrow will be the first working day of his car repair shop. For now the car repair shop is very small and only one car can be repaired at a given time.</p><p>Polycarp is good at marketing, so he has already collected <span class="tex-span"><i>n</i></span> requests from clients. The requests are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in order they came.</p><p>The <span class="tex-span"><i>i</i></span>-th request is characterized by two values: <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> — the day when a client wants to start the repair of his car, <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> — duration (in days) to repair the car. The days are enumerated from 1, the first day is tomorrow, the second day is the day after tomorrow and so on.</p><p>Polycarp is making schedule by processing requests in the order from the first to the <span class="tex-span"><i>n</i></span>-th request. He schedules the <span class="tex-span"><i>i</i></span>-th request as follows:</p><ul> <li> If the car repair shop is idle for <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> days starting from <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub>, <i>s</i><sub class="lower-index"><i>i</i></sub> + 1, ..., <i>s</i><sub class="lower-index"><i>i</i></sub> + <i>d</i><sub class="lower-index"><i>i</i></sub> - 1</span>), then these days are used to repair a car of the <span class="tex-span"><i>i</i></span>-th client. </li><li> Otherwise, Polycarp finds the first day <span class="tex-span"><i>x</i></span> (from 1 and further) that there are <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> subsequent days when no repair is scheduled starting from <span class="tex-span"><i>x</i></span>. In other words he chooses the smallest positive <span class="tex-span"><i>x</i></span> that all days <span class="tex-span"><i>x</i>, <i>x</i> + 1, ..., <i>x</i> + <i>d</i><sub class="lower-index"><i>i</i></sub> - 1</span> are not scheduled for repair of any car. So, the car of the <span class="tex-span"><i>i</i></span>-th client will be repaired in the range <span class="tex-span">[<i>x</i>, <i>x</i> + <i>d</i><sub class="lower-index"><i>i</i></sub> - 1]</span>. It is possible that the day <span class="tex-span"><i>x</i></span> when repair is scheduled to start will be less than <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>. </li></ul><p>Given <span class="tex-span"><i>n</i></span> requests, you are asked to help Polycarp schedule all of them according to the rules above.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200</span>) — the number of requests from clients.</p><p>The following <span class="tex-span"><i>n</i></span> lines contain requests, one request per line. The <span class="tex-span"><i>i</i></span>-th request is given as the pair of integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 5·10<sup class="upper-index">6</sup></span>), where <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> is the preferred time to start repairing the <span class="tex-span"><i>i</i></span>-th car, <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> is the number of days to repair the <span class="tex-span"><i>i</i></span>-th car.</p><p>The requests should be processed in the order they are given in the input.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> lines. The <span class="tex-span"><i>i</i></span>-th line should contain two integers — the start day to repair the <span class="tex-span"><i>i</i></span>-th car and the finish day to repair the <span class="tex-span"><i>i</i></span>-th car.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200</span>) — the number of requests from clients.</p><p>The following <span class="tex-span"><i>n</i></span> lines contain requests, one request per line. The <span class="tex-span"><i>i</i></span>-th request is given as the pair of integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 5·10<sup class="upper-index">6</sup></span>), where <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> is the preferred time to start repairing the <span class="tex-span"><i>i</i></span>-th car, <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> is the number of days to repair the <span class="tex-span"><i>i</i></span>-th car.</p><p>The requests should be processed in the order they are given in the input.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> lines. The <span class="tex-span"><i>i</i></span>-th line should contain two integers — the start day to repair the <span class="tex-span"><i>i</i></span>-th car and the finish day to repair the <span class="tex-span"><i>i</i></span>-th car.</p>





```input1
3
9 2
7 3
2 4

```




```input2
4
1000000000 1000000
1000000000 1000000
100000000 1000000
1000000000 1000000

```




```output1
9 10
1 3
4 7

```




```output2
1000000000 1000999999
1 1000000
100000000 100999999
1000001 2000000

```


