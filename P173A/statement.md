## Description

<div><p>Nikephoros and Polycarpus play rock-paper-scissors. The loser gets pinched (not too severely!).</p><p>Let us remind you the rules of this game. Rock-paper-scissors is played by two players. In each round the players choose one of three items independently from each other. They show the items with their hands: a rock, scissors or paper. The winner is determined by the following rules: the rock beats the scissors, the scissors beat the paper and the paper beats the rock. If the players choose the same item, the round finishes with a draw.</p><p>Nikephoros and Polycarpus have played <span class="tex-span"><i>n</i></span> rounds. In each round the winner gave the loser a friendly pinch and the loser ended up with a fresh and new red spot on his body. If the round finished in a draw, the players did nothing and just played on.</p><p>Nikephoros turned out to have worked out the following strategy: before the game began, he chose some sequence of items <span class="tex-span"><i>A</i> = (<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub>)</span>, and then he cyclically showed the items from this sequence, starting from the first one. Cyclically means that Nikephoros shows signs in the following order: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>m</i></sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>m</i></sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span">...</span> and so on. Polycarpus had a similar strategy, only he had his own sequence of items <span class="tex-span"><i>B</i> = (<i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>k</i></sub>)</span>.</p><p>Determine the number of red spots on both players after they've played <span class="tex-span"><i>n</i></span> rounds of the game. You can consider that when the game began, the boys had no red spots on them.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">9</sup></span>) — the number of the game's rounds.</p><p>The second line contains sequence <span class="tex-span"><i>A</i></span> as a string of <span class="tex-span"><i>m</i></span> characters and the third line contains sequence <span class="tex-span"><i>B</i></span> as a string of <span class="tex-span"><i>k</i></span> characters (<span class="tex-span">1 ≤ <i>m</i>, <i>k</i> ≤ 1000</span>). The given lines only contain characters "<span class="tex-font-style-tt">R</span>", "<span class="tex-font-style-tt">S</span>" and "<span class="tex-font-style-tt">P</span>". Character "<span class="tex-font-style-tt">R</span>" stands for the rock, character "<span class="tex-font-style-tt">S</span>" represents the scissors and "<span class="tex-font-style-tt">P</span>" represents the paper.</p></div><div class="output-specification"><p>Print two space-separated integers: the numbers of red spots Nikephoros and Polycarpus have.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">9</sup></span>) — the number of the game's rounds.</p><p>The second line contains sequence <span class="tex-span"><i>A</i></span> as a string of <span class="tex-span"><i>m</i></span> characters and the third line contains sequence <span class="tex-span"><i>B</i></span> as a string of <span class="tex-span"><i>k</i></span> characters (<span class="tex-span">1 ≤ <i>m</i>, <i>k</i> ≤ 1000</span>). The given lines only contain characters "<span class="tex-font-style-tt">R</span>", "<span class="tex-font-style-tt">S</span>" and "<span class="tex-font-style-tt">P</span>". Character "<span class="tex-font-style-tt">R</span>" stands for the rock, character "<span class="tex-font-style-tt">S</span>" represents the scissors and "<span class="tex-font-style-tt">P</span>" represents the paper.</p>

## Output

<p>Print two space-separated integers: the numbers of red spots Nikephoros and Polycarpus have.</p>





```input1
7
RPS
RSPP

```




```input2
5
RRRRRRRR
R

```




```output1
3 2
```




```output2
0 0
```



## Note

<p>In the first sample the game went like this:</p><ul> <li> <span class="tex-font-style-tt">R - R</span>. Draw. </li><li> <span class="tex-font-style-tt">P - S</span>. Nikephoros loses. </li><li> <span class="tex-font-style-tt">S - P</span>. Polycarpus loses. </li><li> <span class="tex-font-style-tt">R - P</span>. Nikephoros loses. </li><li> <span class="tex-font-style-tt">P - R</span>. Polycarpus loses. </li><li> <span class="tex-font-style-tt">S - S</span>. Draw. </li><li> <span class="tex-font-style-tt">R - P</span>. Nikephoros loses. </li></ul><p>Thus, in total Nikephoros has <span class="tex-span">3</span> losses (and <span class="tex-span">3</span> red spots), and Polycarpus only has <span class="tex-span">2</span>.</p>
