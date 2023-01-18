## Description

<div><p>As we all know, Dart is some kind of creature from Upside Down world. For simplicity, we call their kind <span class="tex-font-style-it">pollywogs</span>. Dart and <span class="tex-span"><i>x</i> - 1</span> other pollywogs are playing a game. There are <span class="tex-span"><i>n</i></span> stones in a row, numbered from <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span> from left to right. At most <span class="tex-span">1</span> pollywog may be sitting on each stone at a time. Initially, the pollywogs are sitting on the first <span class="tex-span"><i>x</i></span> stones (one pollywog on each stone).</p><center> <img class="tex-graphics" src="file://kBVywHxA.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Dart and his friends want to end up on the last <span class="tex-span"><i>x</i></span> stones. At each second, the leftmost pollywog should jump to the right. A pollywog can jump at most <span class="tex-span"><i>k</i></span> stones; more specifically, a pollywog can jump from stone number <span class="tex-span"><i>i</i></span> to stones <span class="tex-span"><i>i</i> + 1, <i>i</i> + 2, ... <i>i</i> + <i>k</i></span>. A pollywog can't jump on an occupied stone. Jumping a distance <span class="tex-span"><i>i</i></span> takes <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> amounts of energy from the pollywog. </p><p>Also, <span class="tex-span"><i>q</i></span> stones are <span class="tex-font-style-it">special</span> Each time landing on a special stone <span class="tex-span"><i>p</i></span>, takes <span class="tex-span"><i>w</i><sub class="lower-index"><i>p</i></sub></span> amounts of energy (in addition to the energy for jump) from the pollywog. <span class="tex-span"><i>w</i><sub class="lower-index"><i>p</i></sub></span> could be negative, in this case, it means the pollywog absorbs <span class="tex-span">|<i>w</i><sub class="lower-index"><i>p</i></sub>|</span> amounts of energy.</p><p>Pollywogs want to spend as little energy as possible (this value could be negative). </p><p>They're just pollywogs, so they asked for your help. Tell them the total change in their energy, in case they move optimally.</p></div><div class="input-specification"><p>The first line of input contains four integers, <span class="tex-span"><i>x</i>, <i>k</i>, <i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>k</i> ≤ 8</span>, <span class="tex-span"><i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">8</sup></span>, <span class="tex-span">0 ≤ <i>q</i> ≤ <i>min</i>(25, <i>n</i> - <i>x</i>)</span>)&nbsp;— the number of pollywogs, the maximum length of jump, the number of stones and the number of special stones.</p><p>The next line contains <span class="tex-span"><i>k</i></span> integers, <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ... <i>c</i><sub class="lower-index"><i>k</i></sub></span>, separated by spaces (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the energetic costs of jumps.</p><p>The next <span class="tex-span"><i>q</i></span> lines contain description of the special stones. Each line contains two integers <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>p</i></sub></span> (<span class="tex-span"><i>x</i> + 1 ≤ <i>p</i> ≤ <i>n</i></span>, <span class="tex-span">|<i>w</i><sub class="lower-index"><i>p</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>). All <span class="tex-span"><i>p</i></span> are distinct.</p></div><div class="output-specification"><p>Print the minimum amount of energy they need, in the first and only line of output.</p></div>

## Input

<p>The first line of input contains four integers, <span class="tex-span"><i>x</i>, <i>k</i>, <i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>k</i> ≤ 8</span>, <span class="tex-span"><i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">8</sup></span>, <span class="tex-span">0 ≤ <i>q</i> ≤ <i>min</i>(25, <i>n</i> - <i>x</i>)</span>)&nbsp;— the number of pollywogs, the maximum length of jump, the number of stones and the number of special stones.</p><p>The next line contains <span class="tex-span"><i>k</i></span> integers, <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ... <i>c</i><sub class="lower-index"><i>k</i></sub></span>, separated by spaces (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the energetic costs of jumps.</p><p>The next <span class="tex-span"><i>q</i></span> lines contain description of the special stones. Each line contains two integers <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>p</i></sub></span> (<span class="tex-span"><i>x</i> + 1 ≤ <i>p</i> ≤ <i>n</i></span>, <span class="tex-span">|<i>w</i><sub class="lower-index"><i>p</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>). All <span class="tex-span"><i>p</i></span> are distinct.</p>

## Output

<p>Print the minimum amount of energy they need, in the first and only line of output.</p>





```input1
2 3 10 2
1 2 3
5 -10
6 1000

```




```input2
4 7 85 3
17 5 28 4 52 46 6
59 -76
33 -69
19 2018

```




```output1
6

```




```output2
135

```


