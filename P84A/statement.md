## Description

<div><p>The hero of our story, Valera, and his best friend Arcady are still in school, and therefore they spend all the free time playing turn-based strategy "GAGA: Go And Go Again". The gameplay is as follows. </p><p>There are two armies on the playing field each of which consists of <span class="tex-span"><i>n</i></span> men (<span class="tex-span"><i>n</i></span> is always even). The current player specifies for each of her soldiers an enemy's soldier he will shoot (a target) and then all the player's soldiers shot simultaneously. This is a game world, and so each soldier shoots perfectly, that is he absolutely always hits the specified target. If an enemy soldier is hit, he will surely die. It may happen that several soldiers had been indicated the same target. Killed soldiers do not participate in the game anymore. </p><p>The game "GAGA" consists of three steps: first Valera makes a move, then Arcady, then Valera again and the game ends. </p><p>You are asked to calculate the maximum total number of soldiers that may be killed during the game. </p></div><div class="input-specification"><p>The input data consist of a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">8</sup></span>, <span class="tex-span"><i>n</i></span> is even). Please note that before the game starts there are <span class="tex-span">2<i>n</i></span> soldiers on the fields. </p></div><div class="output-specification"><p>Print a single number — a maximum total number of soldiers that could be killed in the course of the game in three turns.</p></div>

## Input

<p>The input data consist of a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">8</sup></span>, <span class="tex-span"><i>n</i></span> is even). Please note that before the game starts there are <span class="tex-span">2<i>n</i></span> soldiers on the fields. </p>

## Output

<p>Print a single number — a maximum total number of soldiers that could be killed in the course of the game in three turns.</p>





```input1
2

```




```input2
4

```




```output1
3

```




```output2
6

```



## Note

<p>The first sample test:</p><p>1) Valera's soldiers 1 and 2 shoot at Arcady's soldier 1.</p><p>2) Arcady's soldier 2 shoots at Valera's soldier 1.</p><p>3) Valera's soldier 1 shoots at Arcady's soldier 2.</p><p>There are 3 soldiers killed in total: Valera's soldier 1 and Arcady's soldiers 1 and 2.</p>
