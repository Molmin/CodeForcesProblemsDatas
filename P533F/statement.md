## Description

<div><p>Polycarp invented a new way to encode strings. Let's assume that we have string <span class="tex-span"><i>T</i></span>, consisting of lowercase English letters. Let's choose several pairs of letters of the English alphabet in such a way that each letter occurs in at most one pair. Then let's replace each letter in <span class="tex-span"><i>T</i></span> with its pair letter if there is a pair letter for it. For example, if you chose pairs (<span class="tex-font-style-tt">l</span>, <span class="tex-font-style-tt">r</span>), (<span class="tex-font-style-tt">p</span>, <span class="tex-font-style-tt">q</span>) and (<span class="tex-font-style-tt">a</span>, <span class="tex-font-style-tt">o</span>), then word "<span class="tex-font-style-tt">parallelogram</span>" according to the given encoding principle transforms to word "<span class="tex-font-style-tt">qolorreraglom</span>".</p><p>Polycarpus already has two strings, <span class="tex-span"><i>S</i></span> and <span class="tex-span"><i>T</i></span>. He suspects that string <span class="tex-span"><i>T</i></span> was obtained after applying the given encoding method from some substring of string <span class="tex-span"><i>S</i></span>. Find all positions <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> in <span class="tex-span"><i>S</i></span> (<span class="tex-span">1 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ |<i>S</i>| - |<i>T</i>| + 1</span>), such that <span class="tex-span"><i>T</i></span> can be obtained fro substring <span class="tex-span"><i>S</i><sub class="lower-index"><i>m</i><sub class="lower-index"><i>i</i></sub></sub><i>S</i><sub class="lower-index"><i>m</i><sub class="lower-index"><i>i</i></sub> + 1</sub>... <i>S</i><sub class="lower-index"><i>m</i><sub class="lower-index"><i>i</i></sub> + |<i>T</i>| - 1</sub></span> by applying the described encoding operation by using some set of pairs of English alphabet letters</p></div><div class="input-specification"><p>The first line of the input contains two integers, <span class="tex-span">|<i>S</i>|</span> and <span class="tex-span">|<i>T</i>|</span> (<span class="tex-span">1 ≤ |<i>T</i>| ≤ |<i>S</i>| ≤ 2·10<sup class="upper-index">5</sup></span>) — the lengths of string <span class="tex-span"><i>S</i></span> and string <span class="tex-span"><i>T</i></span>, respectively.</p><p>The second and third line of the input contain strings <span class="tex-span"><i>S</i></span> and <span class="tex-span"><i>T</i></span>, respectively. Both strings consist only of lowercase English letters.</p></div><div class="output-specification"><p>Print number <span class="tex-span"><i>k</i></span> — the number of suitable positions in string <span class="tex-span"><i>S</i></span>.</p><p>In the next line print <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>m</i><sub class="lower-index">1</sub>, <i>m</i><sub class="lower-index">2</sub>, ..., <i>m</i><sub class="lower-index"><i>k</i></sub></span> — the numbers of the suitable positions in the increasing order.</p></div>

## Input

<p>The first line of the input contains two integers, <span class="tex-span">|<i>S</i>|</span> and <span class="tex-span">|<i>T</i>|</span> (<span class="tex-span">1 ≤ |<i>T</i>| ≤ |<i>S</i>| ≤ 2·10<sup class="upper-index">5</sup></span>) — the lengths of string <span class="tex-span"><i>S</i></span> and string <span class="tex-span"><i>T</i></span>, respectively.</p><p>The second and third line of the input contain strings <span class="tex-span"><i>S</i></span> and <span class="tex-span"><i>T</i></span>, respectively. Both strings consist only of lowercase English letters.</p>

## Output

<p>Print number <span class="tex-span"><i>k</i></span> — the number of suitable positions in string <span class="tex-span"><i>S</i></span>.</p><p>In the next line print <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>m</i><sub class="lower-index">1</sub>, <i>m</i><sub class="lower-index">2</sub>, ..., <i>m</i><sub class="lower-index"><i>k</i></sub></span> — the numbers of the suitable positions in the increasing order.</p>





```input1
11 5
abacabadaba
acaba

```




```input2
21 13
paraparallelogramgram
qolorreraglom

```




```output1
3
1 3 7

```




```output2
1
5

```


