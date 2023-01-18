## Description

<div><p>The dragon and the princess are arguing about what to do on the New Year's Eve. The dragon suggests flying to the mountains to watch fairies dancing in the moonlight, while the princess thinks they should just go to bed early. They are desperate to come to an amicable agreement, so they decide to leave this up to chance.</p><p>They take turns drawing a mouse from a bag which initially contains <span class="tex-span"><i>w</i></span> white and <span class="tex-span"><i>b</i></span> black mice. The person who is the first to draw a white mouse wins. After each mouse drawn by the dragon the rest of mice in the bag panic, and one of them jumps out of the bag itself (the princess draws her mice carefully and doesn't scare other mice). <span class="tex-font-style-bf">Princess draws first.</span> What is the probability of the princess winning?</p><p>If there are no more mice in the bag and nobody has drawn a white mouse, the dragon wins. Mice which jump out of the bag themselves are not considered to be drawn (do not define the winner). Once a mouse has left the bag, it never returns to it. Every mouse is drawn from the bag with the same probability as every other one, and every mouse jumps out of the bag with the same probability as every other one.</p></div><div class="input-specification"><p>The only line of input data contains two integers <span class="tex-span"><i>w</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">0 ≤ <i>w</i>, <i>b</i> ≤ 1000</span>).</p></div><div class="output-specification"><p>Output the probability of the princess winning. The answer is considered to be correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p></div>

## Input

<p>The only line of input data contains two integers <span class="tex-span"><i>w</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">0 ≤ <i>w</i>, <i>b</i> ≤ 1000</span>).</p>

## Output

<p>Output the probability of the princess winning. The answer is considered to be correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p>





```input1
1 3

```




```input2
5 5

```




```output1
0.500000000

```




```output2
0.658730159

```



## Note

<p>Let's go through the first sample. The probability of the princess drawing a white mouse on her first turn and winning right away is 1/4. The probability of the dragon drawing a black mouse and not winning on his first turn is 3/4 * 2/3 = 1/2. After this there are two mice left in the bag — one black and one white; one of them jumps out, and the other is drawn by the princess on her second turn. If the princess' mouse is white, she wins (probability is 1/2 * 1/2 = 1/4), otherwise nobody gets the white mouse, so according to the rule the dragon wins.</p>
