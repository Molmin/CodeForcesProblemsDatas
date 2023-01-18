## Description

<div><p>Dark Assembly is a governing body in the Netherworld. Here sit the senators who take the most important decisions for the player. For example, to expand the range of the shop or to improve certain characteristics of the character the Dark Assembly's approval is needed.</p><p>The Dark Assembly consists of <span class="tex-span"><i>n</i></span> senators. Each of them is characterized by his <span class="tex-font-style-it">level</span> and <span class="tex-font-style-it">loyalty</span> to the player. The level is a positive integer which reflects a senator's strength. Loyalty is the probability of a positive decision in the voting, which is measured as a percentage with precision of up to <span class="tex-span">10%</span>. </p><p>Senators make decisions by voting. Each of them makes a positive or negative decision in accordance with their loyalty. If <span class="tex-font-style-bf">strictly more</span> than half of the senators take a positive decision, the player's proposal is approved. </p><p>If the player's proposal is not approved after the voting, then the player may appeal against the decision of the Dark Assembly. To do that, player needs to kill all the senators that voted against (there's nothing wrong in killing senators, they will resurrect later and will treat the player even worse). The probability that a player will be able to kill a certain group of senators is equal to <span class="tex-span"><i>A</i> / (<i>A</i> + <i>B</i>)</span>, where <span class="tex-span"><i>A</i></span> is the sum of levels of all player's characters and <span class="tex-span"><i>B</i></span> is the sum of levels of all senators in this group. If the player kills all undesired senators, then his proposal is approved.</p><p>Senators are very fond of sweets. They can be bribed by giving them candies. For each received candy a senator increases his loyalty to the player by <span class="tex-span">10%</span>. It's worth to mention that loyalty cannot exceed <span class="tex-span">100%</span>. The player can take no more than <span class="tex-span"><i>k</i></span> sweets to the courtroom. Candies should be given to the senators <span class="tex-font-style-bf">before</span> the start of voting.</p><p>Determine the probability that the Dark Assembly approves the player's proposal if the candies are distributed among the senators in the optimal way.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>A</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 8</span>, <span class="tex-span">1 ≤ <i>A</i> ≤ 9999</span>).</p><p>Then <span class="tex-span"><i>n</i></span> lines follow. The <span class="tex-span"><i>i</i></span>-th of them contains two numbers — <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> — the <span class="tex-span"><i>i</i></span>-th senator's level and his loyalty.</p><p>The levels of all senators are integers in range from <span class="tex-span">1</span> to <span class="tex-span">9999</span> (inclusive). The loyalties of all senators are integers in range from <span class="tex-span">0</span> to <span class="tex-span">100</span> (inclusive) and all of them are divisible by <span class="tex-span">10</span>.</p></div><div class="output-specification"><p>Print one real number with precision <span class="tex-span">10<sup class="upper-index"> - 6</sup></span> — the maximal possible probability that the Dark Assembly approves the player's proposal for the best possible distribution of candies among the senators.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>A</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 8</span>, <span class="tex-span">1 ≤ <i>A</i> ≤ 9999</span>).</p><p>Then <span class="tex-span"><i>n</i></span> lines follow. The <span class="tex-span"><i>i</i></span>-th of them contains two numbers — <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> — the <span class="tex-span"><i>i</i></span>-th senator's level and his loyalty.</p><p>The levels of all senators are integers in range from <span class="tex-span">1</span> to <span class="tex-span">9999</span> (inclusive). The loyalties of all senators are integers in range from <span class="tex-span">0</span> to <span class="tex-span">100</span> (inclusive) and all of them are divisible by <span class="tex-span">10</span>.</p>

## Output

<p>Print one real number with precision <span class="tex-span">10<sup class="upper-index"> - 6</sup></span> — the maximal possible probability that the Dark Assembly approves the player's proposal for the best possible distribution of candies among the senators.</p>





```input1
5 6 100
11 80
14 90
23 70
80 30
153 70

```




```input2
5 3 100
11 80
14 90
23 70
80 30
153 70

```




```input3
1 3 20
20 20

```




```output1
1.0000000000

```




```output2
0.9628442962

```




```output3
0.7500000000

```



## Note

<p>In the first sample the best way of candies' distribution is giving them to first three of the senators. It ensures most of votes.</p><p>It the second sample player should give all three candies to the fifth senator.</p>
