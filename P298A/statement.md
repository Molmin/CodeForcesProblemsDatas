## Description

<div><p>There is a straight snowy road, divided into <span class="tex-span"><i>n</i></span> blocks. The blocks are numbered from 1 to <span class="tex-span"><i>n</i></span> from left to right. If one moves from the <span class="tex-span"><i>i</i></span>-th block to the <span class="tex-span">(<i>i</i> + 1)</span>-th block, he will leave a right footprint on the <span class="tex-span"><i>i</i></span>-th block. Similarly, if one moves from the <span class="tex-span"><i>i</i></span>-th block to the <span class="tex-span">(<i>i</i> - 1)</span>-th block, he will leave a left footprint on the <span class="tex-span"><i>i</i></span>-th block. If there already is a footprint on the <span class="tex-span"><i>i</i></span>-th block, the new footprint will cover the old one.</p><center> <img class="tex-graphics" src="file://N0aQeQWH.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>At the beginning, there were no footprints. Then polar bear Alice starts from the <span class="tex-span"><i>s</i></span>-th block, makes a sequence of moves and ends in the <span class="tex-span"><i>t</i></span>-th block. It is known that Alice never moves outside of the road. </p><p>You are given the description of Alice's footprints. Your task is to find a pair of possible values of <span class="tex-span"><i>s</i>, <i>t</i></span> by looking at the footprints.</p></div><div class="input-specification"><p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(3 ≤ <i>n</i> ≤ 1000)</span>.</p><p>The second line contains the description of the road — the string that consists of <span class="tex-span"><i>n</i></span> characters. Each character will be either "<span class="tex-font-style-tt">.</span>" (a block without footprint), or "<span class="tex-font-style-tt">L</span>" (a block with a left footprint), "<span class="tex-font-style-tt">R</span>" (a block with a right footprint).</p><p>It's guaranteed that the given string contains at least one character not equal to "<span class="tex-font-style-tt">.</span>". Also, the first and the last character will always be "<span class="tex-font-style-tt">.</span>". It's guaranteed that a solution exists.</p></div><div class="output-specification"><p>Print two space-separated integers — the values of <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>. If there are several possible solutions you can print any of them.</p></div>

## Input

<p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(3 ≤ <i>n</i> ≤ 1000)</span>.</p><p>The second line contains the description of the road — the string that consists of <span class="tex-span"><i>n</i></span> characters. Each character will be either "<span class="tex-font-style-tt">.</span>" (a block without footprint), or "<span class="tex-font-style-tt">L</span>" (a block with a left footprint), "<span class="tex-font-style-tt">R</span>" (a block with a right footprint).</p><p>It's guaranteed that the given string contains at least one character not equal to "<span class="tex-font-style-tt">.</span>". Also, the first and the last character will always be "<span class="tex-font-style-tt">.</span>". It's guaranteed that a solution exists.</p>

## Output

<p>Print two space-separated integers — the values of <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>. If there are several possible solutions you can print any of them.</p>





```input1
9
..RRLL...

```




```input2
11
.RRRLLLLL..

```




```output1
3 4

```




```output2
7 5

```



## Note

<p>The first test sample is the one in the picture.</p>
