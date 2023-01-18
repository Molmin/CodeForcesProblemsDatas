## Description

<div><p>It's that time of the year when the Russians flood their countryside summer cottages (dachas) and the bus stop has a lot of people. People rarely go to the dacha on their own, it's usually a group, so the people stand in queue by groups.</p><p>The bus stop queue has <span class="tex-span"><i>n</i></span> groups of people. The <span class="tex-span"><i>i</i></span>-th group from the beginning has <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> people. Every <span class="tex-span">30</span> minutes an empty bus arrives at the bus stop, it can carry at most <span class="tex-span"><i>m</i></span> people. Naturally, the people from the first group enter the bus first. Then go the people from the second group and so on. Note that the order of groups in the queue never changes. Moreover, if some group cannot fit all of its members into the current bus, it waits for the next bus together with other groups standing after it in the queue.</p><p>Your task is to determine how many buses is needed to transport all <span class="tex-span"><i>n</i></span> groups to the dacha countryside.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 100)</span>. The next line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i>)</span>.</p></div><div class="output-specification"><p>Print a single integer — the number of buses that is needed to transport all <span class="tex-span"><i>n</i></span> groups to the dacha countryside.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 100)</span>. The next line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i>)</span>.</p>

## Output

<p>Print a single integer — the number of buses that is needed to transport all <span class="tex-span"><i>n</i></span> groups to the dacha countryside.</p>





```input1
4 3
2 3 2 1

```




```input2
3 4
1 2 1

```




```output1
3

```




```output2
1

```


