## Description

<div><p><span class="tex-font-style-it">From beginning till end, this message has been waiting to be conveyed.</span></p><p>For a given unordered multiset of <span class="tex-span"><i>n</i></span> lowercase English letters ("multi" means that a letter may appear more than once), we treat all letters as strings of length <span class="tex-span">1</span>, and repeat the following operation <span class="tex-span"><i>n</i> - 1</span> times:</p><ul> <li> Remove any two elements <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> from the set, and add their concatenation <span class="tex-span"><i>s</i> + <i>t</i></span> to the set. </li></ul><p>The cost of such operation is defined to be <img align="middle" class="tex-formula" src="file://ac03Y2wL.png" style="max-width: 100.0%;max-height: 100.0%;">, where <span class="tex-span"><i>f</i>(<i>s</i>, <i>c</i>)</span> denotes the number of times character <span class="tex-span"><i>c</i></span> appears in string <span class="tex-span"><i>s</i></span>.</p><p>Given a non-negative integer <span class="tex-span"><i>k</i></span>, construct any valid non-empty set of no more than <span class="tex-span">100 000</span> letters, such that the minimum accumulative cost of the whole process is <span class="tex-font-style-bf">exactly</span> <span class="tex-span"><i>k</i></span>. It can be shown that a solution always exists.</p></div><div class="input-specification"><p>The first and only line of input contains a non-negative integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 100 000</span>) — the required minimum cost.</p></div><div class="output-specification"><p>Output a non-empty string of no more than <span class="tex-span">100 000</span> lowercase English letters — any multiset satisfying the requirements, concatenated to be a string.</p><p>Note that the printed string doesn't need to be the final concatenated string. It only needs to represent an unordered multiset of letters.</p></div>

## Input

<p>The first and only line of input contains a non-negative integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 100 000</span>) — the required minimum cost.</p>

## Output

<p>Output a non-empty string of no more than <span class="tex-span">100 000</span> lowercase English letters — any multiset satisfying the requirements, concatenated to be a string.</p><p>Note that the printed string doesn't need to be the final concatenated string. It only needs to represent an unordered multiset of letters.</p>





```input1
12

```




```input2
3

```




```output1
abababab

```




```output2
codeforces

```



## Note

<p>For the multiset {<span class="tex-font-style-tt">'a'</span>, <span class="tex-font-style-tt">'b'</span>, <span class="tex-font-style-tt">'a'</span>, <span class="tex-font-style-tt">'b'</span>, <span class="tex-font-style-tt">'a'</span>, <span class="tex-font-style-tt">'b'</span>, <span class="tex-font-style-tt">'a'</span>, <span class="tex-font-style-tt">'b'</span>}, one of the ways to complete the process is as follows:</p><ul> <li> {<span class="tex-font-style-tt">"ab"</span>, <span class="tex-font-style-tt">"a"</span>, <span class="tex-font-style-tt">"b"</span>, <span class="tex-font-style-tt">"a"</span>, <span class="tex-font-style-tt">"b"</span>, <span class="tex-font-style-tt">"a"</span>, <span class="tex-font-style-tt">"b"</span>}, with a cost of <span class="tex-span">0</span>; </li><li> {<span class="tex-font-style-tt">"aba"</span>, <span class="tex-font-style-tt">"b"</span>, <span class="tex-font-style-tt">"a"</span>, <span class="tex-font-style-tt">"b"</span>, <span class="tex-font-style-tt">"a"</span>, <span class="tex-font-style-tt">"b"</span>}, with a cost of <span class="tex-span">1</span>; </li><li> {<span class="tex-font-style-tt">"abab"</span>, <span class="tex-font-style-tt">"a"</span>, <span class="tex-font-style-tt">"b"</span>, <span class="tex-font-style-tt">"a"</span>, <span class="tex-font-style-tt">"b"</span>}, with a cost of <span class="tex-span">1</span>; </li><li> {<span class="tex-font-style-tt">"abab"</span>, <span class="tex-font-style-tt">"ab"</span>, <span class="tex-font-style-tt">"a"</span>, <span class="tex-font-style-tt">"b"</span>}, with a cost of <span class="tex-span">0</span>; </li><li> {<span class="tex-font-style-tt">"abab"</span>, <span class="tex-font-style-tt">"aba"</span>, <span class="tex-font-style-tt">"b"</span>}, with a cost of <span class="tex-span">1</span>; </li><li> {<span class="tex-font-style-tt">"abab"</span>, <span class="tex-font-style-tt">"abab"</span>}, with a cost of <span class="tex-span">1</span>; </li><li> {<span class="tex-font-style-tt">"abababab"</span>}, with a cost of <span class="tex-span">8</span>. </li></ul><p>The total cost is <span class="tex-span">12</span>, and it can be proved to be the minimum cost of the process.</p>
