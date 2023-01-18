## Description

<div><p>Igor the analyst is at work. He learned about a feature in his text editor called "Replace All". Igor is too bored at work and thus he came up with the following problem:</p><p>Given two strings <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> which consist of the English letters '<span class="tex-font-style-tt">A</span>' and '<span class="tex-font-style-tt">B</span>' only, a pair of strings <span class="tex-span">(<i>s</i>, <i>t</i>)</span> is called <span class="tex-font-style-underline">good</span> if:</p><ul><li> <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> consist of the characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>' only.</li><li> <span class="tex-span">1 ≤ |<i>s</i>|, |<i>t</i>| ≤ <i>n</i></span>, where <span class="tex-span">|<i>z</i>|</span> denotes the length of string <span class="tex-span"><i>z</i></span>, and <span class="tex-span"><i>n</i></span> is a fixed positive integer.</li><li> If we replace all occurrences of '<span class="tex-font-style-tt">A</span>' in <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> with the string <span class="tex-span"><i>s</i></span>, and replace all occurrences of '<span class="tex-font-style-tt">B</span>' in <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> with the string <span class="tex-span"><i>t</i></span>, then the two obtained from <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> strings are equal. </li></ul><p>For example, if <span class="tex-span"><i>x</i> = </span><span class="tex-font-style-tt">AAB</span>, <span class="tex-span"><i>y</i> = </span><span class="tex-font-style-tt">BB</span> and <span class="tex-span"><i>n</i> = 4</span>, then (<span class="tex-font-style-tt">01</span>, <span class="tex-font-style-tt">0101</span>) is one of good pairs of strings, because both obtained after replacing strings are "<span class="tex-font-style-tt">01010101</span>".</p><p>The <span class="tex-font-style-underline">flexibility</span> of a pair of strings <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> is the number of pairs of good strings <span class="tex-span">(<i>s</i>, <i>t</i>)</span>. The pairs are ordered, for example the pairs <span class="tex-span">(</span><span class="tex-font-style-tt">0</span>, <span class="tex-font-style-tt">1</span><span class="tex-span">)</span> and <span class="tex-span">(</span><span class="tex-font-style-tt">1</span>, <span class="tex-font-style-tt">0</span><span class="tex-span">)</span> are different.</p><p>You're given two strings <span class="tex-span"><i>c</i></span> and <span class="tex-span"><i>d</i></span>. They consist of characters '<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">B</span>' and '<span class="tex-font-style-tt">?</span>' only. Find the sum of flexibilities of all possible pairs of strings <span class="tex-span">(<i>c</i>', <i>d</i>')</span> such that <span class="tex-span"><i>c</i>'</span> and <span class="tex-span"><i>d</i>'</span> can be obtained from <span class="tex-span"><i>c</i></span> and <span class="tex-span"><i>d</i></span> respectively by replacing the question marks with either '<span class="tex-font-style-tt">A</span>' or '<span class="tex-font-style-tt">B</span>', modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line contains the string <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ |<i>c</i>| ≤ 3·10<sup class="upper-index">5</sup></span>).</p><p>The second line contains the string <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ |<i>d</i>| ≤ 3·10<sup class="upper-index">5</sup></span>).</p><p>The last line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>).</p></div><div class="output-specification"><p>Output a single integer: the answer to the problem, modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line contains the string <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ |<i>c</i>| ≤ 3·10<sup class="upper-index">5</sup></span>).</p><p>The second line contains the string <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ |<i>d</i>| ≤ 3·10<sup class="upper-index">5</sup></span>).</p><p>The last line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>).</p>

## Output

<p>Output a single integer: the answer to the problem, modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
A?
?
3

```




```input2
A
B
10

```




```output1
2

```




```output2
2046

```



## Note

<p>For the first sample, there are four possible pairs of <span class="tex-span">(<i>c</i>', <i>d</i>')</span>.</p><p>If <span class="tex-span">(<i>c</i>', <i>d</i>') = (</span><span class="tex-font-style-tt">AA</span><span class="tex-span">, </span><span class="tex-font-style-tt">A</span><span class="tex-span">)</span>, then the flexibility is <span class="tex-span">0</span>.</p><p>If <span class="tex-span">(<i>c</i>', <i>d</i>') = (</span><span class="tex-font-style-tt">AB</span><span class="tex-span">, </span><span class="tex-font-style-tt">A</span><span class="tex-span">)</span>, then the flexibility is <span class="tex-span">0</span>.</p><p>If <span class="tex-span">(<i>c</i>', <i>d</i>') = (</span><span class="tex-font-style-tt">AA</span><span class="tex-span">, </span><span class="tex-font-style-tt">B</span><span class="tex-span">)</span>, then the flexibility is <span class="tex-span">2</span>, as the pairs of binary strings <span class="tex-span">(</span><span class="tex-font-style-tt">1</span><span class="tex-span">, </span><span class="tex-font-style-tt">11</span><span class="tex-span">)</span>, <span class="tex-span">(</span><span class="tex-font-style-tt">0</span><span class="tex-span">, </span><span class="tex-font-style-tt">00</span><span class="tex-span">)</span> are the only good pairs.</p><p>If <span class="tex-span">(<i>c</i>', <i>d</i>') = (</span><span class="tex-font-style-tt">AB</span><span class="tex-span">, </span><span class="tex-font-style-tt">B</span><span class="tex-span">)</span>, then the flexibility is <span class="tex-span">0</span>.</p><p>Thus, the total flexibility is <span class="tex-span">2</span>.</p><p>For the second sample, there are <span class="tex-span">2<sup class="upper-index">1</sup> + 2<sup class="upper-index">2</sup> + ... + 2<sup class="upper-index">10</sup> = 2046</span> possible binary strings of length not greater <span class="tex-span">10</span>, and the set of pairs of good strings is precisely the set of pairs <span class="tex-span">(<i>s</i>, <i>s</i>)</span>, where <span class="tex-span"><i>s</i></span> is a binary string of length not greater than <span class="tex-span">10</span>.</p>
