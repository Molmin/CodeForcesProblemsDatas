## Description

<div><p>Little Gennady was presented with a set of domino for his birthday. The set consists of <span class="tex-span">28</span> different dominoes of size <span class="tex-span">2 × 1</span>. Both halves of each domino contain one digit from <span class="tex-span">0</span> to <span class="tex-span">6</span>. </p><pre class="verbatim">0-0 0-1 0-2 0-3 0-4 0-5 0-6<br>1-1 1-2 1-3 1-4 1-5 1-6<br>2-2 2-3 2-4 2-5 2-6<br>3-3 3-4 3-5 3-6<br>4-4 4-5 4-6<br>5-5 5-6<br>6-6<br></pre><p>The figure that consists of <span class="tex-span">28</span> dominoes is called <span class="tex-font-style-underline">magic</span>, if it can be fully covered with <span class="tex-span">14</span> non-intersecting squares of size <span class="tex-span">2 × 2</span> so that each square contained four equal numbers. Every time Gennady assembles a magic figure, some magic properties of the set appear — he wins the next contest. Gennady noticed that he can't assemble a figure that has already been assembled, otherwise someone else wins the contest.</p><center> <img class="tex-graphics" src="file://Py0qASW4.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Gennady chose a checked field of size <span class="tex-span"><i>n</i> × <i>m</i></span> and put there rectangular chips of sizes <span class="tex-span">1 × 2</span> and <span class="tex-span">2 × 1</span>. Each chip fully occupies exactly two neighboring squares of the field. Those chips do not overlap but they can touch each other. Overall the field has exactly <span class="tex-span">28</span> chips, equal to the number of dominoes in the set. Now Gennady wants to replace each chip with a domino so that a magic figure appeared as a result. Different chips should be replaced by different dominoes. Determine in what number of contests Gennady can win over at the given position of the chips. You are also required to find one of the possible ways of replacing chips with dominoes to win the next Codeforces round.</p></div><div class="input-specification"><p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 30</span>). Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters, which is the position of chips on the field. The dots stand for empty spaces, Latin letters from "a" to "z" and "A", "B" stand for the positions of the chips. There are exactly 28 chips on the field. The squares covered by the same chip are marked by the same letter, different chips are marked by different letters. It is guaranteed that the field's description is correct.</p><p>It is also guaranteed that at least one solution exists.</p></div><div class="output-specification"><p>Print on the first line the number of ways to replace chips with dominoes to get a magic figure. That is the total number of contests that can be won using this arrangement of the chips. Next <span class="tex-span"><i>n</i></span> lines containing <span class="tex-span"><i>m</i></span> characters each, should contain a field from dots and numbers from <span class="tex-span">0</span> to <span class="tex-span">6</span> — any of the possible solutions. All dominoes should be different.</p></div>

## Input

<p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 30</span>). Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters, which is the position of chips on the field. The dots stand for empty spaces, Latin letters from "a" to "z" and "A", "B" stand for the positions of the chips. There are exactly 28 chips on the field. The squares covered by the same chip are marked by the same letter, different chips are marked by different letters. It is guaranteed that the field's description is correct.</p><p>It is also guaranteed that at least one solution exists.</p>

## Output

<p>Print on the first line the number of ways to replace chips with dominoes to get a magic figure. That is the total number of contests that can be won using this arrangement of the chips. Next <span class="tex-span"><i>n</i></span> lines containing <span class="tex-span"><i>m</i></span> characters each, should contain a field from dots and numbers from <span class="tex-span">0</span> to <span class="tex-span">6</span> — any of the possible solutions. All dominoes should be different.</p>





```input1
8 8
.aabbcc.
.defghi.
kdefghij
klmnopqj
.lmnopq.
.rstuvw.
xrstuvwy
xzzAABBy

```




```output1
10080
.001122.
.001122.
33440055
33440055
.225566.
.225566.
66113344
66113344

```


