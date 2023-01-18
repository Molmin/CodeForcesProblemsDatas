## Description

<div><p>Recently Polycarp started to develop a text editor that works only with correct bracket sequences (abbreviated as CBS). </p><p>Note that a bracket sequence is correct if it is possible to get a correct mathematical expression by adding "<span class="tex-font-style-tt">+</span>"-s and "<span class="tex-font-style-tt">1</span>"-s to it. For example, sequences "<span class="tex-font-style-tt">(())()</span>", "<span class="tex-font-style-tt">()</span>" and "<span class="tex-font-style-tt">(()(()))</span>" are correct, while "<span class="tex-font-style-tt">)(</span>", "<span class="tex-font-style-tt">(()</span>" and "<span class="tex-font-style-tt">(()))(</span>" are not. Each bracket in CBS has a pair. For example, in "<span class="tex-font-style-tt">(()(()))</span>":</p><ul> <li> 1st bracket is paired with 8th, </li><li> 2d bracket is paired with 3d, </li><li> 3d bracket is paired with 2d, </li><li> 4th bracket is paired with 7th, </li><li> 5th bracket is paired with 6th, </li><li> 6th bracket is paired with 5th, </li><li> 7th bracket is paired with 4th, </li><li> 8th bracket is paired with 1st. </li></ul><p>Polycarp's editor currently supports only three operations during the use of CBS. The cursor in the editor takes the whole position of one of the brackets (not the position between the brackets!). There are three operations being supported:</p><ul> <li> «<span class="tex-font-style-tt">L</span>»&nbsp;— move the cursor one position to the left, </li><li> «<span class="tex-font-style-tt">R</span>»&nbsp;— move the cursor one position to the right, </li><li> «<span class="tex-font-style-tt">D</span>»&nbsp;— delete the bracket in which the cursor is located, delete the bracket it's paired to and all brackets between them (that is, delete a substring between the bracket in which the cursor is located and the one it's paired to). </li></ul><p>After the operation "<span class="tex-font-style-tt">D</span>" the cursor moves to the nearest bracket to the right (of course, among the non-deleted). If there is no such bracket (that is, the suffix of the CBS was deleted), then the cursor moves to the nearest bracket to the left (of course, among the non-deleted). </p><p>There are pictures illustrated several usages of operation "<span class="tex-font-style-tt">D</span>" below.</p><center> <img class="tex-graphics" src="file://ftk4wl4O.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>All incorrect operations (shift cursor over the end of CBS, delete the whole CBS, etc.) are not supported by Polycarp's editor.</p><p>Polycarp is very proud of his development, can you implement the functionality of his editor?</p></div><div class="input-specification"><p>The first line contains three positive integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 500 000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 500 000</span>, <span class="tex-span">1 ≤ <i>p</i> ≤ <i>n</i></span>)&nbsp;— the number of brackets in the correct bracket sequence, the number of operations and the initial position of cursor. Positions in the sequence are numbered from left to right, starting from one. It is guaranteed that <span class="tex-span"><i>n</i></span> is even.</p><p>It is followed by the string of <span class="tex-span"><i>n</i></span> characters "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>" forming the correct bracket sequence.</p><p>Then follow a string of <span class="tex-span"><i>m</i></span> characters "<span class="tex-font-style-tt">L</span>", "<span class="tex-font-style-tt">R</span>" and "<span class="tex-font-style-tt">D</span>"&nbsp;— a sequence of the operations. Operations are carried out one by one from the first to the last. It is guaranteed that the given operations never move the cursor outside the bracket sequence, as well as the fact that after all operations a bracket sequence will be non-empty.</p></div><div class="output-specification"><p>Print the correct bracket sequence, obtained as a result of applying all operations to the initial sequence.</p></div>

## Input

<p>The first line contains three positive integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 500 000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 500 000</span>, <span class="tex-span">1 ≤ <i>p</i> ≤ <i>n</i></span>)&nbsp;— the number of brackets in the correct bracket sequence, the number of operations and the initial position of cursor. Positions in the sequence are numbered from left to right, starting from one. It is guaranteed that <span class="tex-span"><i>n</i></span> is even.</p><p>It is followed by the string of <span class="tex-span"><i>n</i></span> characters "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>" forming the correct bracket sequence.</p><p>Then follow a string of <span class="tex-span"><i>m</i></span> characters "<span class="tex-font-style-tt">L</span>", "<span class="tex-font-style-tt">R</span>" and "<span class="tex-font-style-tt">D</span>"&nbsp;— a sequence of the operations. Operations are carried out one by one from the first to the last. It is guaranteed that the given operations never move the cursor outside the bracket sequence, as well as the fact that after all operations a bracket sequence will be non-empty.</p>

## Output

<p>Print the correct bracket sequence, obtained as a result of applying all operations to the initial sequence.</p>





```input1
8 4 5
(())()()
RDLD

```




```input2
12 5 3
((()())(()))
RRDLD

```




```input3
8 8 8
(())()()
LLLLLLDD

```




```output1
()

```




```output2
(()(()))

```




```output3
()()

```



## Note

<p>In the first sample the cursor is initially at position <span class="tex-span">5</span>. Consider actions of the editor:</p><ol> <li> command "<span class="tex-font-style-tt">R</span>"&nbsp;— the cursor moves to the position <span class="tex-span">6</span> on the right; </li><li> command "<span class="tex-font-style-tt">D</span>"&nbsp;— the deletion of brackets from the position <span class="tex-span">5</span> to the position <span class="tex-span">6</span>. After that CBS takes the form <span class="tex-font-style-tt">(())()</span>, the cursor is at the position <span class="tex-span">5</span>; </li><li> command "<span class="tex-font-style-tt">L</span>"&nbsp;— the cursor moves to the position <span class="tex-span">4</span> on the left; </li><li> command "<span class="tex-font-style-tt">D</span>"&nbsp;— the deletion of brackets from the position <span class="tex-span">1</span> to the position <span class="tex-span">4</span>. After that CBS takes the form <span class="tex-font-style-tt">()</span>, the cursor is at the position <span class="tex-span">1</span>. </li></ol><p>Thus, the answer is equal to <span class="tex-font-style-tt">()</span>.</p>
