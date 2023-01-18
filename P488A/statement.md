## Description

<div><p>Giga Tower is the tallest and deepest building in Cyberland. There are <span class="tex-span">17 777 777 777</span> floors, numbered from <span class="tex-span"> - 8 888 888 888</span> to <span class="tex-span">8 888 888 888</span>. In particular, there is floor <span class="tex-span">0</span> between floor <span class="tex-span"> - 1</span> and floor <span class="tex-span">1</span>. Every day, thousands of tourists come to this place to enjoy the wonderful view. </p><p>In Cyberland, it is believed that the number "8" is a lucky number (that's why Giga Tower has <span class="tex-span">8 888 888 888</span> floors above the ground), and, an integer is <span class="tex-font-style-underline">lucky</span>, if and only if its decimal notation contains at least one digit "8". For example, <span class="tex-span">8,  - 180, 808</span> are all <span class="tex-font-style-underline">lucky</span> while <span class="tex-span">42,  - 10</span> are not. In the Giga Tower, if you write code at a floor with lucky floor number, good luck will always be with you (Well, this round is #278, also lucky, huh?).</p><p>Tourist Henry goes to the tower to seek good luck. Now he is at the floor numbered <span class="tex-span"><i>a</i></span>. He wants to find the minimum <span class="tex-font-style-bf">positive</span> integer <span class="tex-span"><i>b</i></span>, such that, if he walks <span class="tex-span"><i>b</i></span> floors higher, he will arrive at a floor with a <span class="tex-font-style-bf">lucky</span> number. </p></div><div class="input-specification"><p>The only line of input contains an integer <span class="tex-span"><i>a</i></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print the minimum <span class="tex-span"><i>b</i></span> in a line.</p></div>

## Input

<p>The only line of input contains an integer <span class="tex-span"><i>a</i></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print the minimum <span class="tex-span"><i>b</i></span> in a line.</p>





```input1
179

```




```input2
-1

```




```input3
18

```




```output1
1

```




```output2
9

```




```output3
10

```



## Note

<p>For the first sample, he has to arrive at the floor numbered <span class="tex-span">180</span>.</p><p>For the second sample, he will arrive at <span class="tex-span">8</span>.</p><p>Note that <span class="tex-span"><i>b</i></span> should be positive, so the answer for the third sample is <span class="tex-span">10</span>, not <span class="tex-span">0</span>.</p>
