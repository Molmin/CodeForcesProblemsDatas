## Description

<div><p>A sequence of square brackets is regular if by inserting symbols "<span class="tex-font-style-tt">+</span>" and "<span class="tex-font-style-tt">1</span>" into it, you can get a regular mathematical expression from it. For example, sequences "<span class="tex-font-style-tt">[[]][]</span>", "<span class="tex-font-style-tt">[]</span>" and "<span class="tex-font-style-tt">[[][[]]]</span>" — are regular, at the same time "<span class="tex-font-style-tt">][</span>", "<span class="tex-font-style-tt">[[]</span>" and "<span class="tex-font-style-tt">[[]]][</span>" — are irregular. </p><p>Draw the given sequence using a minimalistic pseudographics in the strip of the lowest possible height — use symbols '<span class="tex-font-style-tt">+</span>', '<span class="tex-font-style-tt">-</span>' and '<span class="tex-font-style-tt">|</span>'. For example, the sequence "<span class="tex-font-style-tt">[[][]][]</span>" should be represented as: </p><pre class="verbatim"><br>+-        -++- -+    <br>|+- -++- -+||   |<br>||   ||   |||   |<br>|+- -++- -+||   |<br>+-        -++- -+<br></pre><p>Each bracket should be represented with the hepl of one or more symbols '<span class="tex-font-style-tt">|</span>' (the vertical part) and symbols '<span class="tex-font-style-tt">+</span>' and '<span class="tex-font-style-tt">-</span>' as on the example which is given above.</p><p>Brackets should be drawn without spaces one by one, only dividing pairs of consecutive pairwise brackets with a single-space bar (so that the two brackets do not visually merge into one symbol). The image should have the minimum possible height. </p><p>The enclosed bracket is always smaller than the surrounding bracket, but each bracket separately strives to maximize the height of the image. So the pair of final brackets in the example above occupies the entire height of the image.</p><p>Study carefully the examples below, they adequately explain the condition of the problem. Pay attention that in this problem the answer (the image) is unique. </p></div><div class="input-specification"><p>The first line contains an even integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>) — the length of the sequence of brackets.</p><p>The second line contains the sequence of brackets — these are <span class="tex-span"><i>n</i></span> symbols "<span class="tex-font-style-tt">[</span>" and "<span class="tex-font-style-tt">]</span>". It is guaranteed that the given sequence of brackets is regular. </p></div><div class="output-specification"><p>Print the drawn bracket sequence in the format which is given in the condition. Don't print extra (unnecessary) spaces. </p></div>

## Input

<p>The first line contains an even integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>) — the length of the sequence of brackets.</p><p>The second line contains the sequence of brackets — these are <span class="tex-span"><i>n</i></span> symbols "<span class="tex-font-style-tt">[</span>" and "<span class="tex-font-style-tt">]</span>". It is guaranteed that the given sequence of brackets is regular. </p>

## Output

<p>Print the drawn bracket sequence in the format which is given in the condition. Don't print extra (unnecessary) spaces. </p>





```input1
8
[[][]][]

```




```input2
6
[[[]]]

```




```input3
6
[[][]]

```




```input4
2
[]

```




```input5
4
[][]

```




```output1
+-        -++- -+
|+- -++- -+||   |
||   ||   |||   |
|+- -++- -+||   |
+-        -++- -+

```




```output2
+-     -+
|+-   -+|
||+- -+||
|||   |||
||+- -+||
|+-   -+|
+-     -+

```




```output3
+-        -+
|+- -++- -+|
||   ||   ||
|+- -++- -+|
+-        -+

```




```output4
+- -+
|   |
+- -+

```




```output5
+- -++- -+
|   ||   |
+- -++- -+

```


