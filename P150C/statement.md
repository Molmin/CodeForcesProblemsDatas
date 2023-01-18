## Description

<div><p>I guess there's not much point in reminding you that Nvodsk winters aren't exactly hot. That increased the popularity of the public transport dramatically. The route of bus <span class="tex-span">62</span> has exactly <span class="tex-span"><i>n</i></span> stops (stop <span class="tex-span">1</span> goes first on its way and stop <span class="tex-span"><i>n</i></span> goes last). The stops are positioned on a straight line and their coordinates are <span class="tex-span">0 = <i>x</i><sub class="lower-index">1</sub> &lt; <i>x</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>x</i><sub class="lower-index"><i>n</i></sub></span>. </p><p>Each day exactly <span class="tex-span"><i>m</i></span> people use bus <span class="tex-span">62</span>. For each person we know the number of the stop where he gets on the bus and the number of the stop where he gets off the bus. A ticket from stop <span class="tex-span"><i>a</i></span> to stop <span class="tex-span"><i>b</i></span> (<span class="tex-span"><i>a</i> &lt; <i>b</i></span>) costs <span class="tex-span"><i>x</i><sub class="lower-index"><i>b</i></sub> - <i>x</i><sub class="lower-index"><i>a</i></sub></span> rubles. However, the conductor can choose no more than one segment NOT TO SELL a ticket for. We mean that conductor should choose C and D (С &lt;= D) and sell a ticket for the segments [<span class="tex-span"><i>A</i></span>, <span class="tex-span"><i>C</i></span>] and [<span class="tex-span"><i>D</i></span>, <span class="tex-span"><i>B</i></span>], or not sell the ticket at all. The conductor and the passenger divide the saved money between themselves equally. The conductor's "untaxed income" is sometimes interrupted by inspections that take place as the bus drives on some segment of the route located between two consecutive stops. The inspector fines the conductor by <span class="tex-span"><i>c</i></span> rubles for each passenger who doesn't have the ticket for this route's segment.</p><p>You know the coordinated of all stops <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>; the numbers of stops where the <span class="tex-span"><i>i</i></span>-th passenger gets on and off, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub></span>); the fine <span class="tex-span"><i>c</i></span>; and also <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> — the probability of inspection on segment between the <span class="tex-span"><i>i</i></span>-th and the <span class="tex-span"><i>i</i> + 1</span>-th stop. The conductor asked you to help him make a plan of selling tickets that maximizes the mathematical expectation of his profit.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 150 000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 300 000</span>, <span class="tex-span">1 ≤ <i>c</i> ≤ 10 000</span>).</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = 0</span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> &lt; <i>x</i><sub class="lower-index"><i>i</i> + 1</sub></span>) — the coordinates of the stops on the bus's route.</p><p>The third line contains <span class="tex-span"><i>n</i> - 1</span> integer <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the probability of inspection in percents on the segment between stop <span class="tex-span"><i>i</i></span> and stop <span class="tex-span"><i>i</i> + 1</span>.</p><p>Then follow <span class="tex-span"><i>m</i></span> lines that describe the bus's passengers. Each line contains exactly two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the numbers of stops where the <span class="tex-span"><i>i</i></span>-th passenger gets on and off.</p></div><div class="output-specification"><p>Print the single real number — the maximum expectation of the conductor's profit. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://0htmaWHp.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 150 000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 300 000</span>, <span class="tex-span">1 ≤ <i>c</i> ≤ 10 000</span>).</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = 0</span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> &lt; <i>x</i><sub class="lower-index"><i>i</i> + 1</sub></span>) — the coordinates of the stops on the bus's route.</p><p>The third line contains <span class="tex-span"><i>n</i> - 1</span> integer <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the probability of inspection in percents on the segment between stop <span class="tex-span"><i>i</i></span> and stop <span class="tex-span"><i>i</i> + 1</span>.</p><p>Then follow <span class="tex-span"><i>m</i></span> lines that describe the bus's passengers. Each line contains exactly two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the numbers of stops where the <span class="tex-span"><i>i</i></span>-th passenger gets on and off.</p>

## Output

<p>Print the single real number — the maximum expectation of the conductor's profit. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://0htmaWHp.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
3 3 10
0 10 100
100 0
1 2
2 3
1 3

```




```input2
10 8 187
0 10 30 70 150 310 630 1270 2550 51100
13 87 65 0 100 44 67 3 4
1 10
2 9
3 8
1 5
6 10
2 7
4 10
4 5

```




```output1
90.000000000

```




```output2
76859.990000000

```



## Note

<p>A comment to the first sample:</p><p>The first and third passengers get tickets from stop <span class="tex-span">1</span> to stop <span class="tex-span">2</span>. The second passenger doesn't get a ticket. There always is inspection on the segment <span class="tex-span">1</span>-<span class="tex-span">2</span> but both passengers have the ticket for it. There never is an inspection on the segment <span class="tex-span">2</span>-<span class="tex-span">3</span>, that's why the second passenger gets away with the cheating. Our total profit is <span class="tex-span">(0 + 90 / 2 + 90 / 2) = 90</span>.</p>
