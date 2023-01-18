## Description

<div><p>Andrew and Jerry are playing a game with Harry as the scorekeeper. The game consists of three rounds. In each round, Andrew and Jerry draw randomly without replacement from a jar containing <span class="tex-span"><i>n</i></span> balls, each labeled with a distinct positive integer. Without looking, they hand their balls to Harry, who awards the point to the player with the larger number and <span class="tex-font-style-bf">returns the balls</span> to the jar. The winner of the game is the one who wins at least two of the three rounds.</p><p>Andrew wins rounds 1 and 2 while Jerry wins round 3, so Andrew wins the game. However, Jerry is unhappy with this system, claiming that he will often lose the match despite having the higher overall total. What is the probability that the sum of the three balls Jerry drew is strictly higher than the sum of the three balls Andrew drew?</p></div><div class="input-specification"><p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2000</span>) — the number of balls in the jar.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 5000</span>) — the number written on the <span class="tex-span"><i>i</i></span>th ball. It is guaranteed that no two balls have the same number.</p></div><div class="output-specification"><p>Print a single real value — the probability that Jerry has a higher total, given that Andrew wins the first two rounds and Jerry wins the third. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://X8LsUcz1.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2000</span>) — the number of balls in the jar.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 5000</span>) — the number written on the <span class="tex-span"><i>i</i></span>th ball. It is guaranteed that no two balls have the same number.</p>

## Output

<p>Print a single real value — the probability that Jerry has a higher total, given that Andrew wins the first two rounds and Jerry wins the third. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://X8LsUcz1.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
2
1 2

```




```input2
3
1 2 10

```




```output1
0.0000000000

```




```output2
0.0740740741

```



## Note

<p>In the first case, there are only two balls. In the first two rounds, Andrew must have drawn the <span class="tex-span">2</span> and Jerry must have drawn the <span class="tex-span">1</span>, and vice versa in the final round. Thus, Andrew's sum is <span class="tex-span">5</span> and Jerry's sum is <span class="tex-span">4</span>, so Jerry never has a higher total.</p><p>In the second case, each game could've had three outcomes — <span class="tex-span">10 - 2</span>, <span class="tex-span">10 - 1</span>, or <span class="tex-span">2 - 1</span>. Jerry has a higher total if and only if Andrew won <span class="tex-span">2 - 1</span> in both of the first two rounds, and Jerry drew the <span class="tex-span">10</span> in the last round. This has probability <img align="middle" class="tex-formula" src="file://vhFeaaR2.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
