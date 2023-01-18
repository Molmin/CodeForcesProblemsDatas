## Description

<div><p>Two soldiers are playing a game. At the beginning first of them chooses a positive integer <span class="tex-span"><i>n</i></span> and gives it to the second soldier. Then the second one tries to make maximum possible number of rounds. Each round consists of choosing a positive integer <span class="tex-span"><i>x</i> &gt; 1</span>, such that <span class="tex-span"><i>n</i></span> is divisible by <span class="tex-span"><i>x</i></span> and replacing <span class="tex-span"><i>n</i></span> with <span class="tex-span"><i>n</i> / <i>x</i></span>. When <span class="tex-span"><i>n</i></span> becomes equal to <span class="tex-span">1</span> and there is no more possible valid moves the game is over and the score of the second soldier is equal to the number of rounds he performed.</p><p>To make the game more interesting, first soldier chooses <span class="tex-span"><i>n</i></span> of form <span class="tex-span"><i>a</i>! / <i>b</i>!</span> for some positive integer <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span"><i>a</i> ≥ <i>b</i></span>). Here by <span class="tex-span"><i>k</i>!</span> we denote the <span class="tex-font-style-it">factorial</span> of <span class="tex-span"><i>k</i></span> that is defined as a product of all positive integers not large than <span class="tex-span"><i>k</i></span>.</p><p>What is the maximum possible score of the second soldier?</p></div><div class="input-specification"><p>First line of input consists of single integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 1 000 000</span>) denoting number of games soldiers play.</p><p>Then follow <span class="tex-span"><i>t</i></span> lines, each contains pair of integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>b</i> ≤ <i>a</i> ≤ 5 000 000</span>) defining the value of <span class="tex-span"><i>n</i></span> for a game.</p></div><div class="output-specification"><p>For each game output a maximum score that the second soldier can get.</p></div>

## Input

<p>First line of input consists of single integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 1 000 000</span>) denoting number of games soldiers play.</p><p>Then follow <span class="tex-span"><i>t</i></span> lines, each contains pair of integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>b</i> ≤ <i>a</i> ≤ 5 000 000</span>) defining the value of <span class="tex-span"><i>n</i></span> for a game.</p>

## Output

<p>For each game output a maximum score that the second soldier can get.</p>





```input1
2
3 1
6 3

```




```output1
2
5

```


