## Description

<div><p>Thumbelina has had an accident. She has found herself on a little island in the middle of a swamp and wants to get to the shore very much.</p><p>One can get to the shore only by hills that are situated along a straight line that connects the little island with the shore. Let us assume that the hills are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> and the number of a hill is equal to the distance in meters between it and the island. The distance between the <span class="tex-span"><i>n</i></span>-th hill and the shore is also <span class="tex-span">1</span> meter.</p><p>Thumbelina is too small to make such jumps. Fortunately, a family of frogs living in the swamp suggests to help her. Each frog agrees to give Thumbelina a ride but Thumbelina should choose only one frog. Each frog has a certain jump length. If Thumbelina agrees to accept help from a frog whose jump length is <span class="tex-span"><i>d</i></span>, the frog will jump from the island on the hill <span class="tex-span"><i>d</i></span>, then — on the hill <span class="tex-span">2<i>d</i></span>, then <span class="tex-span">3<i>d</i></span> and so on until they get to the shore (i.e. find itself beyond the hill <span class="tex-span"><i>n</i></span>).</p><p>However, there is one more problem: mosquitoes also live in the swamp. At the moment they have a siesta, and they are having a nap on some hills. If the frog jumps on a hill with a mosquito the frog will smash it. The frogs Thumbelina has met are pacifists, so they will find the death of each mosquito very much sad. Help Thumbelina choose a frog that will bring her to the shore and smash as small number of mosquitoes as possible.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>m</i>, <i>k</i> ≤ 100</span>) — the number of hills, frogs and mosquitoes respectively. The second line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the lengths of the frogs’ jumps. The third line contains <span class="tex-span"><i>k</i></span> integers — the numbers of the hills on which each mosquito is sleeping. No more than one mosquito can sleep on each hill. The numbers in the lines are separated by single spaces.</p></div><div class="output-specification"><p>In the first line output the number of frogs that smash the minimal number of mosquitoes, in the second line — their numbers in increasing order separated by spaces. The frogs are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> in the order of the jump length given in the input data.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>m</i>, <i>k</i> ≤ 100</span>) — the number of hills, frogs and mosquitoes respectively. The second line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the lengths of the frogs’ jumps. The third line contains <span class="tex-span"><i>k</i></span> integers — the numbers of the hills on which each mosquito is sleeping. No more than one mosquito can sleep on each hill. The numbers in the lines are separated by single spaces.</p>

## Output

<p>In the first line output the number of frogs that smash the minimal number of mosquitoes, in the second line — their numbers in increasing order separated by spaces. The frogs are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> in the order of the jump length given in the input data.</p>





```input1
5 3 5
2 3 4
1 2 3 4 5

```




```input2
1000000000 2 3
2 5
999999995 999999998 999999996

```




```output1
2
2 3

```




```output2
1
2

```


