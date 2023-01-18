## Description

<div><p>One day Misha and Andrew were playing a very simple game. First, each player chooses an integer in the range from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Let's assume that Misha chose number <span class="tex-span"><i>m</i></span>, and Andrew chose number <span class="tex-span"><i>a</i></span>.</p><p>Then, by using a random generator they choose a random integer <span class="tex-span"><i>c</i></span> in the range between <span class="tex-span">1</span> and <span class="tex-span"><i>n</i></span> (any integer from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> is chosen with the same probability), after which the winner is the player, whose number was closer to <span class="tex-span"><i>c</i></span>. The boys agreed that if <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>a</i></span> are located on the same distance from <span class="tex-span"><i>c</i></span>, Misha wins.</p><p>Andrew wants to win very much, so he asks you to help him. You know the number selected by Misha, and number <span class="tex-span"><i>n</i></span>. You need to determine which value of <span class="tex-span"><i>a</i></span> Andrew must choose, so that the probability of his victory is the highest possible.</p><p>More formally, you need to find such integer <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ <i>n</i></span>), that the probability that <img align="middle" class="tex-formula" src="file://qQIKjvi2.png" style="max-width: 100.0%;max-height: 100.0%;"> is maximal, where <span class="tex-span"><i>c</i></span> is the equiprobably chosen integer from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> (inclusive).</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>) — the range of numbers in the game, and the number selected by Misha respectively.</p></div><div class="output-specification"><p>Print a single number — such value <span class="tex-span"><i>a</i></span>, that probability that Andrew wins is the highest. If there are multiple such values, print the minimum of them.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>) — the range of numbers in the game, and the number selected by Misha respectively.</p>

## Output

<p>Print a single number — such value <span class="tex-span"><i>a</i></span>, that probability that Andrew wins is the highest. If there are multiple such values, print the minimum of them.</p>





```input1
3 1

```




```input2
4 3

```




```output1
2
```




```output2
2
```



## Note

<p>In the first sample test: Andrew wins if <span class="tex-span"><i>c</i></span> is equal to <span class="tex-span">2</span> or <span class="tex-span">3</span>. The probability that Andrew wins is <span class="tex-span">2 / 3</span>. If Andrew chooses <span class="tex-span"><i>a</i> = 3</span>, the probability of winning will be <span class="tex-span">1 / 3</span>. If <span class="tex-span"><i>a</i> = 1</span>, the probability of winning is <span class="tex-span">0</span>.</p><p>In the second sample test: Andrew wins if <span class="tex-span"><i>c</i></span> is equal to <span class="tex-span">1</span> and <span class="tex-span">2</span>. The probability that Andrew wins is <span class="tex-span">1 / 2</span>. For other choices of <span class="tex-span"><i>a</i></span> the probability of winning is less.</p>
