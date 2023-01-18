## Description

<div><p>This year Alex has finished school, and now he is a first-year student of Berland State University. For him it was a total surprise that even though he studies programming, he still has to attend physical education lessons. The end of the term is very soon, but, unfortunately, Alex still hasn't attended a single lesson!</p><p>Since Alex doesn't want to get expelled, he wants to know the number of working days left until the end of the term, so he can attend physical education lessons during these days. But in BSU calculating the number of working days is a complicated matter:</p><p>There are <span class="tex-span"><i>n</i></span> days left before the end of the term (numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>), and initially all of them are working days. Then the university staff sequentially publishes <span class="tex-span"><i>q</i></span> orders, one after another. Each order is characterised by three numbers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>k</i></span>:</p><ul> <li> If <span class="tex-span"><i>k</i> = 1</span>, then all days from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span> (inclusive) become non-working days. If some of these days are made working days by some previous order, then these days still become non-working days; </li><li> If <span class="tex-span"><i>k</i> = 2</span>, then all days from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span> (inclusive) become working days. If some of these days are made non-working days by some previous order, then these days still become working days. </li></ul><p>Help Alex to determine the number of working days left after each order!</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span>, and the second line — one integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the number of days left before the end of the term, and the number of orders, respectively.</p><p>Then <span class="tex-span"><i>q</i></span> lines follow, <span class="tex-span"><i>i</i></span>-th line containing three integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> representing <span class="tex-span"><i>i</i></span>-th order (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>).</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>q</i></span> integers. <span class="tex-span"><i>i</i></span>-th of them must be equal to the number of working days left until the end of the term after the first <span class="tex-span"><i>i</i></span> orders are published.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span>, and the second line — one integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the number of days left before the end of the term, and the number of orders, respectively.</p><p>Then <span class="tex-span"><i>q</i></span> lines follow, <span class="tex-span"><i>i</i></span>-th line containing three integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> representing <span class="tex-span"><i>i</i></span>-th order (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>).</p>

## Output

<p>Print <span class="tex-span"><i>q</i></span> integers. <span class="tex-span"><i>i</i></span>-th of them must be equal to the number of working days left until the end of the term after the first <span class="tex-span"><i>i</i></span> orders are published.</p>





```input1
4
6
1 2 1
3 4 1
2 3 2
1 3 2
2 4 1
1 4 2

```




```output1
2
0
2
3
1
4

```


