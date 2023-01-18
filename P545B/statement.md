## Description

<div><p>Little Susie loves strings. Today she calculates distances between them. As Susie is a small girl after all, her strings contain only digits zero and one. She uses the definition of Hamming distance:</p><p>We will define the distance between two strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> of the same length consisting of digits zero and one as the number of positions <span class="tex-span"><i>i</i></span>, such that <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> isn't equal to <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>. </p><p>As besides everything else Susie loves symmetry, she wants to find for two strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> of length <span class="tex-span"><i>n</i></span> such string <span class="tex-span"><i>p</i></span> of length <span class="tex-span"><i>n</i></span>, that the distance from <span class="tex-span"><i>p</i></span> to <span class="tex-span"><i>s</i></span> was equal to the distance from <span class="tex-span"><i>p</i></span> to <span class="tex-span"><i>t</i></span>.</p><p>It's time for Susie to go to bed, help her find such string <span class="tex-span"><i>p</i></span> or state that it is impossible.</p></div><div class="input-specification"><p>The first line contains string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span>. </p><p>The second line contains string <span class="tex-span"><i>t</i></span> of length <span class="tex-span"><i>n</i></span>.</p><p>The length of string <span class="tex-span"><i>n</i></span> is within range from <span class="tex-span">1</span> to <span class="tex-span">10<sup class="upper-index">5</sup></span>. It is guaranteed that both strings contain only digits zero and one.</p></div><div class="output-specification"><p>Print a string of length <span class="tex-span"><i>n</i></span>, consisting of digits zero and one, that meets the problem statement. If no such string exist, print on a single line "impossible" (without the quotes).</p><p>If there are multiple possible answers, print any of them.</p></div>

## Input

<p>The first line contains string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span>. </p><p>The second line contains string <span class="tex-span"><i>t</i></span> of length <span class="tex-span"><i>n</i></span>.</p><p>The length of string <span class="tex-span"><i>n</i></span> is within range from <span class="tex-span">1</span> to <span class="tex-span">10<sup class="upper-index">5</sup></span>. It is guaranteed that both strings contain only digits zero and one.</p>

## Output

<p>Print a string of length <span class="tex-span"><i>n</i></span>, consisting of digits zero and one, that meets the problem statement. If no such string exist, print on a single line "impossible" (without the quotes).</p><p>If there are multiple possible answers, print any of them.</p>





```input1
0001
1011

```




```input2
000
111

```




```output1
0011

```




```output2
impossible

```



## Note

<p>In the first sample different answers are possible, namely — 0010, 0011, 0110, 0111, 1000, 1001, 1100, 1101.</p>
