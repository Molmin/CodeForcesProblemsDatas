## Description

<div><p>Farmer John is hosting a tennis tournament with his <span class="tex-span"><i>n</i></span> cows. Each cow has a skill level <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>, and no two cows having the same skill level. Every cow plays every other cow exactly once in the tournament, and each cow beats every cow with skill level lower than its own.</p><p>However, Farmer John thinks the tournament will be demoralizing for the weakest cows who lose most or all of their matches, so he wants to flip some of the results. In particular, at <span class="tex-span"><i>k</i></span> different instances, he will take two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> and flip all the results between cows with skill level between <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> inclusive. That is, for any pair <span class="tex-span"><i>x</i>, <i>y</i></span> <img align="middle" class="tex-formula" src="file://csFf0Rqr.png" style="max-width: 100.0%;max-height: 100.0%;"> he will change the result of the match on the final scoreboard (so if <span class="tex-span"><i>x</i></span> won the match, the scoreboard will now display that <span class="tex-span"><i>y</i></span> won the match, and vice versa). It is possible that Farmer John will change the result of a match multiple times. It is not guaranteed that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are equal to some cow's skill level.</p><p>Farmer John wants to determine how balanced he made the tournament results look. In particular, he wants to count the number of triples of cows <span class="tex-span">(<i>p</i>, <i>q</i>, <i>r</i>)</span> for which the final leaderboard shows that cow <span class="tex-span"><i>p</i></span> beats cow <span class="tex-span"><i>q</i></span>, cow <span class="tex-span"><i>q</i></span> beats cow <span class="tex-span"><i>r</i></span>, and cow <span class="tex-span"><i>r</i></span> beats cow <span class="tex-span"><i>p</i></span>. Help him determine this number.</p><p>Note that two triples are considered different if they do not contain the same set of cows (i.e. if there is a cow in one triple that is not in the other).</p></div><div class="input-specification"><p>On the first line are two space-separated integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;0 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup>)</span>. On the next line are <span class="tex-span"><i>n</i></span> space-separated distinct integers, <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>, denoting the skill levels of the cows. On the next <span class="tex-span"><i>k</i></span> lines are two space separated integers, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> representing the changes Farmer John made to the scoreboard in the order he makes it.</p></div><div class="output-specification"><p>A single integer, containing the number of triples of cows <span class="tex-span">(<i>p</i>, <i>q</i>, <i>r</i>)</span> for which the final leaderboard shows that cow <span class="tex-span"><i>p</i></span> beats cow <span class="tex-span"><i>q</i></span>, cow <span class="tex-span"><i>q</i></span> beats cow <span class="tex-span"><i>r</i></span>, and cow <span class="tex-span"><i>r</i></span> beats cow <span class="tex-span"><i>p</i></span>.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>On the first line are two space-separated integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;0 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup>)</span>. On the next line are <span class="tex-span"><i>n</i></span> space-separated distinct integers, <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>, denoting the skill levels of the cows. On the next <span class="tex-span"><i>k</i></span> lines are two space separated integers, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> representing the changes Farmer John made to the scoreboard in the order he makes it.</p>

## Output

<p>A single integer, containing the number of triples of cows <span class="tex-span">(<i>p</i>, <i>q</i>, <i>r</i>)</span> for which the final leaderboard shows that cow <span class="tex-span"><i>p</i></span> beats cow <span class="tex-span"><i>q</i></span>, cow <span class="tex-span"><i>q</i></span> beats cow <span class="tex-span"><i>r</i></span>, and cow <span class="tex-span"><i>r</i></span> beats cow <span class="tex-span"><i>p</i></span>.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
3 2
1 2 3
1 2
2 3

```




```input2
5 3
5 9 4 1 7
1 7
2 8
3 9

```




```output1
1

```




```output2
3

```



## Note

<p>In the first sample, cow 3 &gt; cow 1, cow 3 &gt; cow 2, and cow 2 &gt; cow 1. However, the results between cows 1 and 2 and cows 2 and 3 are flipped, so now FJ's results show that cow 1 &gt; cow 2, cow 2 &gt; cow 3, and cow 3 &gt; cow 1, so cows 1, 2, and 3 form a balanced triple. </p>
