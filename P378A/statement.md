## Description

<div><p>Two players are playing a game. First each of them writes an integer from 1 to 6, and then a dice is thrown. The player whose written number got closer to the number on the dice wins. If both payers have the same difference, it's a draw.</p><p>The first player wrote number <span class="tex-span"><i>a</i></span>, the second player wrote number <span class="tex-span"><i>b</i></span>. How many ways to throw a dice are there, at which the first player wins, or there is a draw, or the second player wins?</p></div><div class="input-specification"><p>The single line contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 6</span>)&nbsp;— the numbers written on the paper by the first and second player, correspondingly.</p></div><div class="output-specification"><p>Print three integers: the number of ways to throw the dice at which the first player wins, the game ends with a draw or the second player wins, correspondingly.</p></div>

## Input

<p>The single line contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 6</span>)&nbsp;— the numbers written on the paper by the first and second player, correspondingly.</p>

## Output

<p>Print three integers: the number of ways to throw the dice at which the first player wins, the game ends with a draw or the second player wins, correspondingly.</p>





```input1
2 5

```




```input2
2 4

```




```output1
3 0 3

```




```output2
2 1 3

```



## Note

<p>The dice is a standard cube-shaped six-sided object with each side containing a number from 1 to 6, and where all numbers on all sides are distinct.</p><p>You can assume that number <span class="tex-span"><i>a</i></span> is closer to number <span class="tex-span"><i>x</i></span> than number <span class="tex-span"><i>b</i></span>, if <span class="tex-span">|<i>a</i> - <i>x</i>| &lt; |<i>b</i> - <i>x</i>|</span>.</p>
