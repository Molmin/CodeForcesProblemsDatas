## Description

<div><p><span class="tex-font-style-it">Notice that the memory limit is non-standard.</span></p><p>Recently Arthur and Sasha have studied correct bracket sequences. Arthur understood this topic perfectly and become so amazed about correct bracket sequences, so he even got himself a favorite correct bracket sequence of length <span class="tex-span">2<i>n</i></span>. Unlike Arthur, Sasha understood the topic very badly, and broke Arthur's favorite correct bracket sequence just to spite him.</p><p>All Arthur remembers about his favorite sequence is for each opening parenthesis ('<span class="tex-font-style-tt">(</span>') the approximate distance to the corresponding closing one ('<span class="tex-font-style-tt">)</span>'). For the <span class="tex-span"><i>i</i></span>-th opening bracket he remembers the segment <span class="tex-span">[<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>]</span>, containing the distance to the corresponding closing bracket.</p><p>Formally speaking, for the <span class="tex-span"><i>i</i></span>-th opening bracket (in order from left to right) we know that the difference of its position and the position of the corresponding closing bracket belongs to the segment <span class="tex-span">[<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>]</span>.</p><p>Help Arthur restore his favorite correct bracket sequence!</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 600</span>), the number of opening brackets in Arthur's favorite correct bracket sequence. </p><p>Next <span class="tex-span"><i>n</i></span> lines contain numbers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> &lt; 2<i>n</i></span>), representing the segment where lies the distance from the <span class="tex-span"><i>i</i></span>-th opening bracket and the corresponding closing one. </p><p>The descriptions of the segments are given in the order in which the opening brackets occur in Arthur's favorite sequence if we list them from left to right.</p></div><div class="output-specification"><p>If it is possible to restore the correct bracket sequence by the given data, print any possible choice.</p><p>If Arthur got something wrong, and there are no sequences corresponding to the given information, print a single line "<span class="tex-font-style-tt">IMPOSSIBLE</span>" (without the quotes).</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 600</span>), the number of opening brackets in Arthur's favorite correct bracket sequence. </p><p>Next <span class="tex-span"><i>n</i></span> lines contain numbers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> &lt; 2<i>n</i></span>), representing the segment where lies the distance from the <span class="tex-span"><i>i</i></span>-th opening bracket and the corresponding closing one. </p><p>The descriptions of the segments are given in the order in which the opening brackets occur in Arthur's favorite sequence if we list them from left to right.</p>

## Output

<p>If it is possible to restore the correct bracket sequence by the given data, print any possible choice.</p><p>If Arthur got something wrong, and there are no sequences corresponding to the given information, print a single line "<span class="tex-font-style-tt">IMPOSSIBLE</span>" (without the quotes).</p>





```input1
4
1 1
1 1
1 1
1 1

```




```input2
3
5 5
3 3
1 1

```




```input3
3
5 5
3 3
2 2

```




```input4
3
2 3
1 4
1 4

```




```output1
()()()()

```




```output2
((()))

```




```output3
IMPOSSIBLE

```




```output4
(())()

```


