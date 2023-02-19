## Description

<div><p>Misha and Vanya have played several table tennis sets. Each set consists of several serves, each serve is won by one of the players, he receives one point and the loser receives nothing. Once one of the players scores exactly <span class="tex-span"><i>k</i></span> points, the score is reset and a new set begins.</p><p>Across all the sets Misha scored <span class="tex-span"><i>a</i></span> points in total, and Vanya scored <span class="tex-span"><i>b</i></span> points. Given this information, determine the maximum number of sets they could have played, or that the situation is impossible.</p><p>Note that the game consisted of several complete sets.</p></div><div class="input-specification"><p>The first line contains three space-separated integers <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>a</i> + <i>b</i> &gt; 0</span>).</p></div><div class="output-specification"><p>If the situation is impossible, print a single number -1. Otherwise, print the maximum possible number of sets.</p></div>

## Input

<p>The first line contains three space-separated integers <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>a</i> + <i>b</i> &gt; 0</span>).</p>

## Output

<p>If the situation is impossible, print a single number -1. Otherwise, print the maximum possible number of sets.</p>





```input1
11 11 5

```




```input2
11 2 3

```




```output1
1

```




```output2
-1

```



## Note

<p>Note that the rules of the game in this problem differ from the real table tennis game, for example, the rule of "balance" (the winning player has to be at least two points ahead to win a set) has no power within the present problem.</p>
