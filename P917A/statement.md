## Description

<div><p>As Will is stuck in the Upside Down, he can still communicate with his mom, Joyce, through the Christmas lights (he can turn them on and off with his mind). He can't directly tell his mom where he is, because the monster that took him to the Upside Down will know and relocate him. </p><center> <img class="tex-graphics" src="file://lZmZ5SyK.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Thus, he came up with a puzzle to tell his mom his coordinates. His coordinates are the answer to the following problem.</p><p>A string consisting only of parentheses ('<span class="tex-font-style-tt">(</span>' and '<span class="tex-font-style-tt">)</span>') is called a bracket sequence. Some bracket sequence are called correct bracket sequences. More formally:</p><ul> <li> Empty string is a correct bracket sequence. </li><li> if <span class="tex-span"><i>s</i></span> is a correct bracket sequence, then <span class="tex-span">(<i>s</i>)</span> is also a correct bracket sequence. </li><li> if <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> are correct bracket sequences, then <span class="tex-span"><i>st</i></span> (concatenation of <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>) is also a correct bracket sequence. </li></ul><p>A string consisting of parentheses and question marks ('<span class="tex-font-style-tt">?</span>') is called pretty if and only if there's a way to replace each question mark with either '<span class="tex-font-style-tt">(</span>' or '<span class="tex-font-style-tt">)</span>' such that the resulting string is a <span class="tex-font-style-bf">non-empty</span> correct bracket sequence.</p><p>Will gave his mom a string <span class="tex-span"><i>s</i></span> consisting of parentheses and question marks (using Morse code through the lights) and his coordinates are the number of pairs of integers <span class="tex-span">(<i>l</i>, <i>r</i>)</span> such that <span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ |<i>s</i>|</span> and the string <span class="tex-span"><i>s</i><sub class="lower-index"><i>l</i></sub><i>s</i><sub class="lower-index"><i>l</i> + 1</sub>... <i>s</i><sub class="lower-index"><i>r</i></sub></span> is pretty, where <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> is <span class="tex-span"><i>i</i></span>-th character of <span class="tex-span"><i>s</i></span>.</p><p>Joyce doesn't know anything about bracket sequences, so she asked for your help.</p></div><div class="input-specification"><p>The first and only line of input contains string <span class="tex-span"><i>s</i></span>, consisting only of characters '<span class="tex-font-style-tt">(</span>', '<span class="tex-font-style-tt">)</span>' and '<span class="tex-font-style-tt">?</span>' (<span class="tex-span">2 ≤ |<i>s</i>| ≤ 5000</span>).</p></div><div class="output-specification"><p>Print the answer to Will's puzzle in the first and only line of output.</p></div>

## Input

<p>The first and only line of input contains string <span class="tex-span"><i>s</i></span>, consisting only of characters '<span class="tex-font-style-tt">(</span>', '<span class="tex-font-style-tt">)</span>' and '<span class="tex-font-style-tt">?</span>' (<span class="tex-span">2 ≤ |<i>s</i>| ≤ 5000</span>).</p>

## Output

<p>Print the answer to Will's puzzle in the first and only line of output.</p>





```input1
((?))

```




```input2
??()??

```




```output1
4

```




```output2
7

```



## Note

<p>For the first sample testcase, the pretty substrings of <span class="tex-span"><i>s</i></span> are:</p><ol> <li> "<span class="tex-font-style-tt">(?</span>" which can be transformed to "<span class="tex-font-style-tt">()</span>". </li><li> "<span class="tex-font-style-tt">?)</span>" which can be transformed to "<span class="tex-font-style-tt">()</span>". </li><li> "<span class="tex-font-style-tt">((?)</span>" which can be transformed to "<span class="tex-font-style-tt">(())</span>". </li><li> "<span class="tex-font-style-tt">(?))</span>" which can be transformed to "<span class="tex-font-style-tt">(())</span>". </li></ol> <p>For the second sample testcase, the pretty substrings of <span class="tex-span"><i>s</i></span> are:</p><ol> <li> "<span class="tex-font-style-tt">??</span>" which can be transformed to "<span class="tex-font-style-tt">()</span>". </li><li> "<span class="tex-font-style-tt">()</span>". </li><li> "<span class="tex-font-style-tt">??()</span>" which can be transformed to "<span class="tex-font-style-tt">()()</span>". </li><li> "<span class="tex-font-style-tt">?()?</span>" which can be transformed to "<span class="tex-font-style-tt">(())</span>". </li><li> "<span class="tex-font-style-tt">??</span>" which can be transformed to "<span class="tex-font-style-tt">()</span>". </li><li> "<span class="tex-font-style-tt">()??</span>" which can be transformed to "<span class="tex-font-style-tt">()()</span>". </li><li> "<span class="tex-font-style-tt">??()??</span>" which can be transformed to "<span class="tex-font-style-tt">()()()</span>". </li></ol>
