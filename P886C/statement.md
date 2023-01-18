## Description

<div><p>A very brave explorer Petya once decided to explore Paris catacombs. Since Petya is not really experienced, his exploration is just walking through the catacombs.</p><p>Catacombs consist of several rooms and bidirectional passages between some pairs of them. Some passages can connect a room to itself and since the passages are built on different depths they do not intersect each other. Every minute Petya arbitrary chooses a passage from the room he is currently in and then reaches the room on the other end of the passage in exactly one minute. When he enters a room at minute <span class="tex-span"><i>i</i></span>, he makes a note in his logbook with number <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>: </p><ul> <li> If Petya has visited this room before, he writes down the minute he was in this room last time; </li><li> Otherwise, Petya writes down an arbitrary non-negative integer strictly less than current minute <span class="tex-span"><i>i</i></span>. </li></ul><p>Initially, Petya was in one of the rooms at minute <span class="tex-span">0</span>, he didn't write down number <span class="tex-span"><i>t</i><sub class="lower-index">0</sub></span>.</p><p>At some point during his wandering Petya got tired, threw out his logbook and went home. Vasya found his logbook and now he is curious: what is the minimum possible number of rooms in Paris catacombs according to Petya's logbook?</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — then number of notes in Petya's logbook.</p><p>The second line contains <span class="tex-span"><i>n</i></span> non-negative integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i></span>) — notes in the logbook.</p></div><div class="output-specification"><p>In the only line print a single integer — the minimum possible number of rooms in Paris catacombs.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — then number of notes in Petya's logbook.</p><p>The second line contains <span class="tex-span"><i>n</i></span> non-negative integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i></span>) — notes in the logbook.</p>

## Output

<p>In the only line print a single integer — the minimum possible number of rooms in Paris catacombs.</p>





```input1
2
0 0

```




```input2
5
0 1 0 1 3

```




```output1
2

```




```output2
3

```



## Note

<p>In the first sample, sequence of rooms Petya visited could be, for example <span class="tex-span">1 → 1 → 2</span>, <span class="tex-span">1 → 2 → 1</span> or <span class="tex-span">1 → 2 → 3</span>. The minimum possible number of rooms is <span class="tex-span">2</span>.</p><p>In the second sample, the sequence could be <span class="tex-span">1 → 2 → 3 → 1 → 2 → 1</span>.</p>
