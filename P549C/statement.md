## Description

<div><p>There are <span class="tex-span"><i>n</i></span> cities in Westeros. The <span class="tex-span"><i>i</i></span>-th city is inhabited by <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> people. Daenerys and Stannis play the following game: in one single move, a player chooses a certain town and burns it to the ground. Thus all its residents, sadly, die. Stannis starts the game. The game ends when Westeros has exactly <span class="tex-span"><i>k</i></span> cities left.</p><p>The prophecy says that if the total number of surviving residents is even, then Daenerys wins: Stannis gets beheaded, and Daenerys rises on the Iron Throne. If the total number of surviving residents is odd, Stannis wins and everything goes in the completely opposite way.</p><p>Lord Petyr Baelish wants to know which candidates to the throne he should support, and therefore he wonders, which one of them has a winning strategy. Answer to this question of Lord Baelish and maybe you will become the next Lord of Harrenholl.</p></div><div class="input-specification"><p>The first line contains two positive space-separated integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the initial number of cities in Westeros and the number of cities at which the game ends. </p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated positive integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>), which represent the population of each city in Westeros.</p></div><div class="output-specification"><p>Print string "<span class="tex-font-style-tt">Daenerys</span>" (without the quotes), if Daenerys wins and "<span class="tex-font-style-tt">Stannis</span>" (without the quotes), if Stannis wins.</p></div>

## Input

<p>The first line contains two positive space-separated integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the initial number of cities in Westeros and the number of cities at which the game ends. </p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated positive integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>), which represent the population of each city in Westeros.</p>

## Output

<p>Print string "<span class="tex-font-style-tt">Daenerys</span>" (without the quotes), if Daenerys wins and "<span class="tex-font-style-tt">Stannis</span>" (without the quotes), if Stannis wins.</p>





```input1
3 1
1 2 1

```




```input2
3 1
2 2 1

```




```input3
6 3
5 20 12 7 14 101

```




```output1
Stannis

```




```output2
Daenerys

```




```output3
Stannis

```



## Note

<p>In the first sample Stannis will use his move to burn a city with two people and Daenerys will be forced to burn a city with one resident. The only survivor city will have one resident left, that is, the total sum is odd, and thus Stannis wins.</p><p>In the second sample, if Stannis burns a city with two people, Daenerys burns the city with one resident, or vice versa. In any case, the last remaining city will be inhabited by two people, that is, the total sum is even, and hence Daenerys wins.</p>
