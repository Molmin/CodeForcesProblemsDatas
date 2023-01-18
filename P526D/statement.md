## Description

<div><p>One day Om Nom found a thread with <span class="tex-span"><i>n</i></span> beads of different colors. He decided to cut the first several beads from this thread to make a bead necklace and present it to his girlfriend Om Nelly.</p><center> <img class="tex-graphics" src="file://qNhdQyHo.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Om Nom knows that his girlfriend loves beautiful patterns. That's why he wants the beads on the necklace to form a <span class="tex-font-style-it">regular</span> pattern. A sequence of beads <span class="tex-span"><i>S</i></span> is <span class="tex-font-style-it">regular</span> if it can be represented as <span class="tex-span"><i>S</i> = <i>A</i> + <i>B</i> + <i>A</i> + <i>B</i> + <i>A</i> + ... + <i>A</i> + <i>B</i> + <i>A</i></span>, where <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> are some bead sequences, "<span class="tex-span"> + </span>" is the concatenation of sequences, there are exactly <span class="tex-span">2<i>k</i> + 1</span> summands in this sum, among which there are <span class="tex-span"><i>k</i> + 1</span> "<span class="tex-span"><i>A</i></span>" summands and <span class="tex-span"><i>k</i></span> "<span class="tex-span"><i>B</i></span>" summands that follow in alternating order. Om Nelly knows that her friend is an eager mathematician, so she doesn't mind if <span class="tex-span"><i>A</i></span> or <span class="tex-span"><i>B</i></span> is an empty sequence.</p><p>Help Om Nom determine in which ways he can cut off the first several beads from the found thread (at least one; probably, all) so that they form a <span class="tex-font-style-it">regular pattern</span>. When Om Nom cuts off the beads, he doesn't change their order.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 1 000 000</span>) — the number of beads on the thread that Om Nom found and number <span class="tex-span"><i>k</i></span> from the definition of the regular sequence above.</p><p>The second line contains the sequence of <span class="tex-span"><i>n</i></span> lowercase Latin letters that represent the colors of the beads. Each color corresponds to a single letter.</p></div><div class="output-specification"><p>Print a string consisting of <span class="tex-span"><i>n</i></span> zeroes and ones. Position <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) must contain either number one if the first <span class="tex-span"><i>i</i></span> beads on the thread form a regular sequence, or a zero otherwise.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 1 000 000</span>) — the number of beads on the thread that Om Nom found and number <span class="tex-span"><i>k</i></span> from the definition of the regular sequence above.</p><p>The second line contains the sequence of <span class="tex-span"><i>n</i></span> lowercase Latin letters that represent the colors of the beads. Each color corresponds to a single letter.</p>

## Output

<p>Print a string consisting of <span class="tex-span"><i>n</i></span> zeroes and ones. Position <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) must contain either number one if the first <span class="tex-span"><i>i</i></span> beads on the thread form a regular sequence, or a zero otherwise.</p>





```input1
7 2
bcabcab

```




```input2
21 2
ababaababaababaababaa

```




```output1
0000011
```




```output2
000110000111111000011
```



## Note

<p>In the first sample test a regular sequence is both a sequence of the first 6 beads (we can take <span class="tex-span"><i>A</i> = </span>"", <span class="tex-span"><i>B</i> = </span>"<span class="tex-font-style-tt">bca</span>"), and a sequence of the first 7 beads (we can take <span class="tex-span"><i>A</i> = </span>"<span class="tex-font-style-tt">b</span>", <span class="tex-span"><i>B</i> = </span>"<span class="tex-font-style-tt">ca</span>").</p><p>In the second sample test, for example, a sequence of the first 13 beads is regular, if we take <span class="tex-span"><i>A</i> = </span>"<span class="tex-font-style-tt">aba</span>", <span class="tex-span"><i>B</i> = </span>"<span class="tex-font-style-tt">ba</span>".</p>
