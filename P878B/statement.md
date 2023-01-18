## Description

<div><p>This time the Berland Team Olympiad in Informatics is held in a remote city that can only be reached by one small bus. Bus has <span class="tex-span"><i>n</i></span> passenger seats, seat <span class="tex-span"><i>i</i></span> can be occupied only by a participant from the city <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Today the bus has completed <span class="tex-span"><i>m</i></span> trips, each time bringing <span class="tex-span"><i>n</i></span> participants. The participants were then aligned in one line in the order they arrived, with people from the same bus standing in the order of their seats (i.&nbsp;e. if we write down the cities where the participants came from, we get the sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> repeated <span class="tex-span"><i>m</i></span> times).</p><p>After that some teams were formed, each consisting of <span class="tex-span"><i>k</i></span> participants form the same city standing next to each other in the line. Once formed, teams left the line. The teams were formed until there were no <span class="tex-span"><i>k</i></span> neighboring participants from the same city.</p><p>Help the organizers determine how many participants have left in the line after that process ended. We can prove that answer doesn't depend on the order in which teams were selected.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i>, <i>k</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">2 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of city, person from which must take seat <span class="tex-span"><i>i</i></span> in the bus. </p></div><div class="output-specification"><p>Output the number of remaining participants in the line.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i>, <i>k</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">2 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of city, person from which must take seat <span class="tex-span"><i>i</i></span> in the bus. </p>

## Output

<p>Output the number of remaining participants in the line.</p>





```input1
4 2 5
1 2 3 1

```




```input2
1 9 10
1

```




```input3
3 2 10
1 2 1

```




```output1
12

```




```output2
1

```




```output3
0

```



## Note

<p>In the second example, the line consists of ten participants from the same city. Nine of them will form a team. At the end, only one participant will stay in the line.</p>
