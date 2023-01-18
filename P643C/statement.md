## Description

<div><p>Radewoosh is playing a computer game. There are <span class="tex-span"><i>n</i></span> levels, numbered <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span>. Levels are divided into <span class="tex-span"><i>k</i></span> regions (groups). Each region contains some positive number of consecutive levels.</p><p>The game repeats the the following process:</p><ol><li> If all regions are beaten then the game ends immediately. Otherwise, the system finds the first region with at least one non-beaten level. Let <span class="tex-span"><i>X</i></span> denote this region.</li><li> The system creates an empty bag for tokens. Each token will represent one level and there may be many tokens representing the same level.<ul> <li> For each already beaten level <span class="tex-span"><i>i</i></span> in the region <span class="tex-span"><i>X</i></span>, the system adds <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> tokens to the bag (tokens representing the <span class="tex-span"><i>i</i></span>-th level). </li><li> Let <span class="tex-span"><i>j</i></span> denote the first non-beaten level in the region <span class="tex-span"><i>X</i></span>. The system adds <span class="tex-span"><i>t</i><sub class="lower-index"><i>j</i></sub></span> tokens to the bag. </li></ul></li><li> Finally, the system takes a uniformly random token from the bag and a player starts the level represented by the token. A player spends one hour and beats the level, even if he has already beaten it in the past. </li></ol><p>Given <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and values <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span>, your task is to split levels into regions. Each level must belong to exactly one region, and each region must contain non-empty consecutive set of levels. What is the minimum possible expected number of hours required to finish the game?</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>min</i>(50, <i>n</i>)</span>)&nbsp;— the number of levels and the number of regions, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>).</p></div><div class="output-specification"><p>Print one real number&nbsp;— the minimum possible expected value of the number of hours spent to finish the game if levels are distributed between regions in the optimal way. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct if <img align="middle" class="tex-formula" src="file://nrA5b99o.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>min</i>(50, <i>n</i>)</span>)&nbsp;— the number of levels and the number of regions, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>).</p>

## Output

<p>Print one real number&nbsp;— the minimum possible expected value of the number of hours spent to finish the game if levels are distributed between regions in the optimal way. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct if <img align="middle" class="tex-formula" src="file://nrA5b99o.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
4 2
100 3 5 7

```




```input2
6 2
1 2 4 8 16 32

```




```output1
5.7428571429

```




```output2
8.5000000000

```



## Note

<p>In the first sample, we are supposed to split <span class="tex-span">4</span> levels into <span class="tex-span">2</span> regions. It's optimal to create the first region with only one level (it must be the first level). Then, the second region must contain other three levels.</p><p>In the second sample, it's optimal to split levels into two regions with <span class="tex-span">3</span> levels each.</p>
