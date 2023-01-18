## Description

<div><p>Johnny is at a carnival which has <span class="tex-span"><i>n</i></span> raffles. Raffle <span class="tex-span"><i>i</i></span> has a prize with value <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>. Each participant can put tickets in whichever raffles they choose (they may have more than one ticket in a single raffle). At the end of the carnival, one ticket is selected at random from each raffle, and the owner of the ticket wins the associated prize. A single person can win multiple prizes from different raffles. </p><p>However, county rules prevent any one participant from owning more than half the tickets in a single raffle, i.e. putting more tickets in the raffle than all the other participants combined. To help combat this (and possibly win some prizes), the organizers started by placing a single ticket in each raffle, which they will never remove.</p><p>Johnny bought <span class="tex-span"><i>t</i></span> tickets and is wondering where to place them. Currently, there are a total of <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> tickets in the <span class="tex-span"><i>i</i></span>-th raffle. He watches as other participants place tickets and modify their decisions and, at every moment in time, wants to know how much he can possibly earn. Find the maximum possible expected value of Johnny's winnings at each moment if he distributes his tickets optimally. Johnny may redistribute all of his tickets arbitrarily between each update, but he may not place more than <span class="tex-span"><i>t</i></span> tickets total or have more tickets in a single raffle than all other participants combined.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>t</i></span>, and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>t</i>, <i>q</i> ≤ 200 000</span>) — the number of raffles, the number of tickets Johnny has, and the total number of updates, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — the value of the <span class="tex-span"><i>i</i></span>-th prize.</p><p>The third line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — the number of tickets initially in the <span class="tex-span"><i>i</i></span>-th raffle.</p><p>The last <span class="tex-span"><i>q</i></span> lines contain the descriptions of the updates. Each description contains two integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>k</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>k</i></sub> ≤ 2</span>, <span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i></span>) — the type of the update and the raffle number. An update of type <span class="tex-span">1</span> represents another participant adding a ticket to raffle <span class="tex-span"><i>r</i><sub class="lower-index"><i>k</i></sub></span>. An update of type <span class="tex-span">2</span> represents another participant removing a ticket from raffle <span class="tex-span"><i>r</i><sub class="lower-index"><i>k</i></sub></span>.</p><p>It is guaranteed that, after each update, each raffle has at least <span class="tex-span">1</span> ticket (not including Johnny's) in it.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>q</i></span> lines, each containing a single real number&nbsp;— the maximum expected value of Johnny's winnings after the <span class="tex-span"><i>k</i></span>-th update. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://ZKqA1XOA.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>t</i></span>, and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>t</i>, <i>q</i> ≤ 200 000</span>) — the number of raffles, the number of tickets Johnny has, and the total number of updates, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — the value of the <span class="tex-span"><i>i</i></span>-th prize.</p><p>The third line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — the number of tickets initially in the <span class="tex-span"><i>i</i></span>-th raffle.</p><p>The last <span class="tex-span"><i>q</i></span> lines contain the descriptions of the updates. Each description contains two integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>k</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>k</i></sub> ≤ 2</span>, <span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i></span>) — the type of the update and the raffle number. An update of type <span class="tex-span">1</span> represents another participant adding a ticket to raffle <span class="tex-span"><i>r</i><sub class="lower-index"><i>k</i></sub></span>. An update of type <span class="tex-span">2</span> represents another participant removing a ticket from raffle <span class="tex-span"><i>r</i><sub class="lower-index"><i>k</i></sub></span>.</p><p>It is guaranteed that, after each update, each raffle has at least <span class="tex-span">1</span> ticket (not including Johnny's) in it.</p>

## Output

<p>Print <span class="tex-span"><i>q</i></span> lines, each containing a single real number&nbsp;— the maximum expected value of Johnny's winnings after the <span class="tex-span"><i>k</i></span>-th update. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://ZKqA1XOA.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
2 1 3
4 5
1 2
1 1
1 2
2 1

```




```input2
3 20 5
6 8 10
6 6 6
1 1
1 2
1 3
2 3
2 3

```




```output1
1.666666667
1.333333333
2.000000000

```




```output2
12.000000000
12.000000000
11.769230769
12.000000000
12.000000000

```



## Note

<p>In the first case, Johnny only has one ticket to distribute. The prizes are worth <span class="tex-span">4</span> and <span class="tex-span">5</span>, and the raffles initially have <span class="tex-span">1</span> and <span class="tex-span">2</span> tickets, respectively. After the first update, each raffle has <span class="tex-span">2</span> tickets, so Johnny has expected value <img align="middle" class="tex-formula" src="file://lNZpuC1e.png" style="max-width: 100.0%;max-height: 100.0%;"> of winning by placing his ticket into the second raffle. The second update adds a ticket to the second raffle, so Johnny can win <img align="middle" class="tex-formula" src="file://Br3vx8ns.png" style="max-width: 100.0%;max-height: 100.0%;"> in the first raffle. After the final update, Johnny keeps his ticket in the first raffle and wins <img align="middle" class="tex-formula" src="file://c5xdMVDm.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>In the second case, Johnny has more tickets than he is allowed to spend. In particular, after the first update, there are <span class="tex-span">7</span>, <span class="tex-span">6</span>, and <span class="tex-span">6</span> tickets in each raffle, respectively, so Johnny can only put in <span class="tex-span">19</span> tickets, winning each prize with probability <img align="middle" class="tex-formula" src="file://D9Eai0aR.png" style="max-width: 100.0%;max-height: 100.0%;">. Also, note that after the last two updates, Johnny must remove a ticket from the last raffle in order to stay under <img align="middle" class="tex-formula" src="file://ptkOVmeB.png" style="max-width: 100.0%;max-height: 100.0%;"> the tickets in the third raffle.</p>
