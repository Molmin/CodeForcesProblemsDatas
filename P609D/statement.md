## Description

<div><p>Nura wants to buy <span class="tex-span"><i>k</i></span> gadgets. She has only <span class="tex-span"><i>s</i></span> burles for that. She can buy each gadget for dollars or for pounds. So each gadget is selling only for some type of currency. The type of currency and the cost in that currency are not changing.</p><p>Nura can buy gadgets for <span class="tex-span"><i>n</i></span> days. For each day you know the exchange rates of dollar and pound, so you know the cost of conversion burles to dollars or to pounds.</p><p>Each day (from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>) Nura can buy some gadgets by current exchange rate. Each day she can buy any gadgets she wants, but each gadget can be bought no more than once during <span class="tex-span"><i>n</i></span> days.</p><p>Help Nura to find the minimum day index when she will have <span class="tex-span"><i>k</i></span> gadgets. Nura always pays with burles, which are converted according to the exchange rate of the purchase day. Nura can't buy dollars or pounds, she always stores only burles. Gadgets are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> in order of their appearing in input.</p></div><div class="input-specification"><p>First line contains four integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i>, <i>s</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup>, 1 ≤ <i>k</i> ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup>, 1 ≤ <i>s</i> ≤ 10<sup class="upper-index">9</sup></span>) — number of days, total number and required number of gadgets, number of burles Nura has.</p><p>Second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the cost of one dollar in burles on <span class="tex-span"><i>i</i></span>-th day.</p><p>Third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the cost of one pound in burles on <span class="tex-span"><i>i</i></span>-th day.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2, 1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — type of the gadget and it's cost. For the gadgets of the first type cost is specified in dollars. For the gadgets of the second type cost is specified in pounds.</p></div><div class="output-specification"><p>If Nura can't buy <span class="tex-span"><i>k</i></span> gadgets print the only line with the number <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise the first line should contain integer <span class="tex-span"><i>d</i></span> — the minimum day index, when Nura will have <span class="tex-span"><i>k</i></span> gadgets. On each of the next <span class="tex-span"><i>k</i></span> lines print two integers <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub></span> — the number of gadget and the day gadget should be bought. All values <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> should be different, but the values <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> can coincide (so Nura can buy several gadgets at one day). The days are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p><p>In case there are multiple possible solutions, print any of them.</p></div>

## Input

<p>First line contains four integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i>, <i>s</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup>, 1 ≤ <i>k</i> ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup>, 1 ≤ <i>s</i> ≤ 10<sup class="upper-index">9</sup></span>) — number of days, total number and required number of gadgets, number of burles Nura has.</p><p>Second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the cost of one dollar in burles on <span class="tex-span"><i>i</i></span>-th day.</p><p>Third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the cost of one pound in burles on <span class="tex-span"><i>i</i></span>-th day.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2, 1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — type of the gadget and it's cost. For the gadgets of the first type cost is specified in dollars. For the gadgets of the second type cost is specified in pounds.</p>

## Output

<p>If Nura can't buy <span class="tex-span"><i>k</i></span> gadgets print the only line with the number <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise the first line should contain integer <span class="tex-span"><i>d</i></span> — the minimum day index, when Nura will have <span class="tex-span"><i>k</i></span> gadgets. On each of the next <span class="tex-span"><i>k</i></span> lines print two integers <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub></span> — the number of gadget and the day gadget should be bought. All values <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> should be different, but the values <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> can coincide (so Nura can buy several gadgets at one day). The days are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p><p>In case there are multiple possible solutions, print any of them.</p>





```input1
5 4 2 2
1 2 3 2 1
3 2 1 2 3
1 1
2 1
1 2
2 2

```




```input2
4 3 2 200
69 70 71 72
104 105 106 107
1 1
2 2
1 2

```




```input3
4 3 1 1000000000
900000 910000 940000 990000
990000 999000 999900 999990
1 87654
2 76543
1 65432

```




```output1
3
1 1
2 3

```




```output2
-1

```




```output3
-1

```


