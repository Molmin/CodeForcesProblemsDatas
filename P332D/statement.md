## Description

<div><p>Insurgents accidentally got hold of the plan of a top secret research polygon created on a distant planet for the needs of the Galaxy Empire. The insurgents suppose that this polygon is developing new deadly weapon. The polygon consists of <span class="tex-span"><i>n</i></span> missile silos connected by bidirectional underground passages. The passages are linked to laboratories where research is conducted. Naturally, the passages are guarded severely: the passage between silos <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> is patrolled by <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> war droids.</p><p>The insurgents studied the polygon plan and noticed its unusual structure. As it turned out, for any <span class="tex-span"><i>k</i></span>-element set of silos <span class="tex-span"><i>S</i></span> there is exactly one silo that is directly connected by a passage with each silo from <span class="tex-span"><i>S</i></span> (we'll call this silo <span class="tex-font-style-underline">adjacent with <span class="tex-span"><i>S</i></span></span>). Having considered that, the insurgents decided to act as follows:</p><ol> <li> they choose a <span class="tex-span"><i>k</i></span>-element set of silos <span class="tex-span"><i>S</i></span>; </li><li> a group of scouts lands from the air into each silo from <span class="tex-span"><i>S</i></span>; </li><li> each group moves along the corresponding passage to the silo, adjacent with <span class="tex-span"><i>S</i></span> (as the scouts move, they check out the laboratories and watch for any signs of weapon blueprints); </li><li> in the silo, adjacent with <span class="tex-span"><i>S</i></span>, the groups get on the ship and fly away. </li></ol><p><span class="tex-font-style-underline">The danger of the operation</span> is the total number of droids that patrol the passages through which the scouts will go. The danger of the operation obviously only depends on the way to choose set <span class="tex-span"><i>S</i></span>. The insurgents haven't yet decided on the exact silos to send the scouts to. However, they already want to start preparing the weapons for the scout groups. To do that, the insurgents need to know the mathematical average of the dangers of the operations that correspond to all possible ways to choose set <span class="tex-span"><i>S</i></span>. Solve this problem to help the insurgents protect the ideals of the Republic!</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> - 1</span>) — the number of silos and the number of scout groups, correspondingly. The next <span class="tex-span"><i>n</i> - 1</span> lines describe the polygon plan: the <span class="tex-span"><i>i</i></span>-th of these lines contains <span class="tex-span"><i>n</i> - <i>i</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i>, <i>i</i> + 1</sub>, <i>c</i><sub class="lower-index"><i>i</i>, <i>i</i> + 2</sub>, ..., <i>c</i><sub class="lower-index"><i>i</i>, <i>n</i></sub></span> — the number of droids that patrol the corresponding passages (-<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>; if <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = </span> -<span class="tex-span">1</span>, then silos <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> don't have a passage between them). All passages are bidirectional, that is, we can assume that <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = <i>c</i><sub class="lower-index"><i>j</i>, <i>i</i></sub></span>. No passages connect a silo with itself. It is guaranteed that the polygon plan meets the conditions of the problem statement.</p></div><div class="output-specification"><p>Print the average danger of the scouting operation, <span class="tex-font-style-bf">rounded down to an integer</span>. Note that at the given limits the answer to the problem <span class="tex-font-style-bf">always</span> fits into the standard integer 64-bit data type.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cout</span> stream or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> - 1</span>) — the number of silos and the number of scout groups, correspondingly. The next <span class="tex-span"><i>n</i> - 1</span> lines describe the polygon plan: the <span class="tex-span"><i>i</i></span>-th of these lines contains <span class="tex-span"><i>n</i> - <i>i</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i>, <i>i</i> + 1</sub>, <i>c</i><sub class="lower-index"><i>i</i>, <i>i</i> + 2</sub>, ..., <i>c</i><sub class="lower-index"><i>i</i>, <i>n</i></sub></span> — the number of droids that patrol the corresponding passages (-<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>; if <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = </span> -<span class="tex-span">1</span>, then silos <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> don't have a passage between them). All passages are bidirectional, that is, we can assume that <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = <i>c</i><sub class="lower-index"><i>j</i>, <i>i</i></sub></span>. No passages connect a silo with itself. It is guaranteed that the polygon plan meets the conditions of the problem statement.</p>

## Output

<p>Print the average danger of the scouting operation, <span class="tex-font-style-bf">rounded down to an integer</span>. Note that at the given limits the answer to the problem <span class="tex-font-style-bf">always</span> fits into the standard integer 64-bit data type.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cout</span> stream or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
6 1
-1 -1 -1 8 -1
-1 5 -1 -1
-1 -1 3
-1 -1
-1

```




```input2
3 2
10 0
11

```




```output1
5

```




```output2
14

```



## Note

<p>In the first sample there are 6 one-element sets of silos. For sets <span class="tex-span">{1}</span>, <span class="tex-span">{5}</span> the operation danger will equal 8, for sets <span class="tex-span">{3}</span>, <span class="tex-span">{6}</span> — 3, for sets <span class="tex-span">{2}</span>, <span class="tex-span">{4}</span> — 5. The mathematical average equals <img align="middle" class="tex-formula" src="file://bfr2xc2s.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>In the second sample there are 3 two-elements sets of silos: <span class="tex-span">{1, 3}</span> (danger equals 21), <span class="tex-span">{1, 2}</span> (danger equals 11), <span class="tex-span">{2, 3}</span> (danger equals 10). The average operation danger equals <img align="middle" class="tex-formula" src="file://JvfuGlul.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
