## Description

<div><p>Yaroslav is playing a game called "Time". The game has a timer showing the lifespan he's got left. As soon as the timer shows 0, Yaroslav's character dies and the game ends. Also, the game has <span class="tex-span"><i>n</i></span> clock stations, station number <span class="tex-span"><i>i</i></span> is at point <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> of the plane. As the player visits station number <span class="tex-span"><i>i</i></span>, he increases the current time on his timer by <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. The stations are for one-time use only, so if the player visits some station another time, the time on his timer won't grow.</p><p>A player spends <span class="tex-span"><i>d</i>·<i>dist</i></span> time units to move between stations, where <span class="tex-span"><i>dist</i></span> is the distance the player has covered and <span class="tex-span"><i>d</i></span> is some constant. The distance between stations <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> is determined as <span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub> - <i>x</i><sub class="lower-index"><i>j</i></sub>| + |<i>y</i><sub class="lower-index"><i>i</i></sub> - <i>y</i><sub class="lower-index"><i>j</i></sub>|</span>.</p><p>Initially, the player is at station number <span class="tex-span">1</span>, and the player has strictly more than zero and strictly less than one units of time. At station number <span class="tex-span">1</span> one unit of money can increase the time on the timer by one time unit (you can buy only integer number of time units).</p><p>Now Yaroslav is wondering, how much money he needs to get to station <span class="tex-span"><i>n</i></span>. Help Yaroslav. Consider the time to buy and to increase the timer value negligibly small.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>d</i></span> <span class="tex-span">(3 ≤ <i>n</i> ≤ 100, 10<sup class="upper-index">3</sup> ≤ <i>d</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of stations and the constant from the statement.</p><p>The second line contains <span class="tex-span"><i>n</i> - 2</span> integers: <span class="tex-span"><i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">3</sup>)</span>. The next <span class="tex-span"><i>n</i></span> lines contain the coordinates of the stations. The <span class="tex-span"><i>i</i></span>-th of them contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(</span>-<span class="tex-span">100 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span>.</p><p>It is guaranteed that no two stations are located at the same point.</p></div><div class="output-specification"><p>In a single line print an integer — the answer to the problem.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>d</i></span> <span class="tex-span">(3 ≤ <i>n</i> ≤ 100, 10<sup class="upper-index">3</sup> ≤ <i>d</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of stations and the constant from the statement.</p><p>The second line contains <span class="tex-span"><i>n</i> - 2</span> integers: <span class="tex-span"><i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">3</sup>)</span>. The next <span class="tex-span"><i>n</i></span> lines contain the coordinates of the stations. The <span class="tex-span"><i>i</i></span>-th of them contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(</span>-<span class="tex-span">100 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span>.</p><p>It is guaranteed that no two stations are located at the same point.</p>

## Output

<p>In a single line print an integer — the answer to the problem.</p>





```input1
3 1000
1000
0 0
0 1
0 3

```




```input2
3 1000
1000
1 0
1 1
1 2

```




```output1
2000

```




```output2
1000

```


