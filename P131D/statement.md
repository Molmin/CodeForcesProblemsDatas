## Description

<div><p>A subway scheme, classic for all Berland cities is represented by a set of <span class="tex-span"><i>n</i></span> stations connected by <span class="tex-span"><i>n</i></span> passages, each of which connects exactly two stations and does not pass through any others. Besides, in the classic scheme one can get from any station to any other one along the passages. The passages can be used to move in both directions. Between each pair of stations there is no more than one passage.</p><p>Berland mathematicians have recently proved a theorem that states that any classic scheme has a ringroad. There can be only one ringroad. In other words, in any classic scheme one can find the only scheme consisting of stations (where any two neighbouring ones are linked by a passage) and this cycle doesn't contain any station more than once.</p><p>This invention had a powerful social impact as now the stations could be compared according to their distance from the ringroad. For example, a citizen could say "I live in three passages from the ringroad" and another one could reply "you loser, I live in one passage from the ringroad". The Internet soon got filled with applications that promised to count the distance from the station to the ringroad (send a text message to a short number...).</p><p>The Berland government decided to put an end to these disturbances and start to control the situation. You are requested to write a program that can determine the remoteness from the ringroad for each station by the city subway scheme.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 3000</span>), <span class="tex-span"><i>n</i></span> is the number of stations (and trains at the same time) in the subway scheme. Then <span class="tex-span"><i>n</i></span> lines contain descriptions of the trains, one per line. Each line contains a pair of integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) and represents the presence of a passage from station <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> to station <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>. The stations are numbered from 1 to <span class="tex-span"><i>n</i></span> in an arbitrary order. It is guaranteed that <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub></span> and that no pair of stations contain more than one passage. The passages can be used to travel both ways. It is guaranteed that the given description represents a classic subway scheme.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> numbers. Separate the numbers by spaces, the <span class="tex-span"><i>i</i></span>-th one should be equal to the distance of the <span class="tex-span"><i>i</i></span>-th station from the ringroad. For the ringroad stations print number <span class="tex-font-style-tt">0</span>.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 3000</span>), <span class="tex-span"><i>n</i></span> is the number of stations (and trains at the same time) in the subway scheme. Then <span class="tex-span"><i>n</i></span> lines contain descriptions of the trains, one per line. Each line contains a pair of integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) and represents the presence of a passage from station <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> to station <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>. The stations are numbered from 1 to <span class="tex-span"><i>n</i></span> in an arbitrary order. It is guaranteed that <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub></span> and that no pair of stations contain more than one passage. The passages can be used to travel both ways. It is guaranteed that the given description represents a classic subway scheme.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> numbers. Separate the numbers by spaces, the <span class="tex-span"><i>i</i></span>-th one should be equal to the distance of the <span class="tex-span"><i>i</i></span>-th station from the ringroad. For the ringroad stations print number <span class="tex-font-style-tt">0</span>.</p>





```input1
4
1 3
4 3
4 2
1 2

```




```input2
6
1 2
3 4
6 4
2 3
1 3
3 5

```




```output1
0 0 0 0
```




```output2
0 0 0 1 1 2
```


