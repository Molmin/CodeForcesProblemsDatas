## Description

<div><p>You are given a string <span class="tex-span"><i>s</i></span> consisting of <span class="tex-span"><i>n</i></span> lowercase Latin letters.</p><p>Let's denote <span class="tex-span"><i>k</i></span>-substring of <span class="tex-span"><i>s</i></span> as a string <span class="tex-span"><i>subs</i><sub class="lower-index"><i>k</i></sub> = <i>s</i><sub class="lower-index"><i>k</i></sub><i>s</i><sub class="lower-index"><i>k</i> + 1</sub>..<i>s</i><sub class="lower-index"><i>n</i> + 1 - <i>k</i></sub></span>. Obviously, <span class="tex-span"><i>subs</i><sub class="lower-index">1</sub> = <i>s</i></span>, and there are exactly <img align="middle" class="tex-formula" src="file://iTyZrBvR.png" style="max-width: 100.0%;max-height: 100.0%;"> such substrings.</p><p>Let's call some string <span class="tex-span"><i>t</i></span> an <span class="tex-font-style-bf">odd proper suprefix</span> of a string <span class="tex-span"><i>T</i></span> iff the following conditions are met:</p><ul><li> <span class="tex-span">|<i>T</i>| &gt; |<i>t</i>|</span>; </li><li> <span class="tex-span">|<i>t</i>|</span> is an odd number; </li><li> <span class="tex-span"><i>t</i></span> is simultaneously a prefix and a suffix of <span class="tex-span"><i>T</i></span>.</li></ul><p>For evey <span class="tex-span"><i>k</i></span>-substring (<img align="middle" class="tex-formula" src="file://jgImvzwo.png" style="max-width: 100.0%;max-height: 100.0%;">) of <span class="tex-span"><i>s</i></span> you have to calculate the maximum length of its odd proper suprefix.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span> — the length <span class="tex-span"><i>s</i></span>.</p><p>The second line contains the string <span class="tex-span"><i>s</i></span> consisting of <span class="tex-span"><i>n</i></span> lowercase Latin letters.</p></div><div class="output-specification"><p>Print <img align="middle" class="tex-formula" src="file://BHXtHcWA.png" style="max-width: 100.0%;max-height: 100.0%;"> integers. <span class="tex-span"><i>i</i></span>-th of them should be equal to maximum length of an odd proper suprefix of <span class="tex-span"><i>i</i></span>-substring of <span class="tex-span"><i>s</i></span> (or <span class="tex-span"> - 1</span>, if there is no such string that is an odd proper suprefix of <span class="tex-span"><i>i</i></span>-substring).</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span> — the length <span class="tex-span"><i>s</i></span>.</p><p>The second line contains the string <span class="tex-span"><i>s</i></span> consisting of <span class="tex-span"><i>n</i></span> lowercase Latin letters.</p>

## Output

<p>Print <img align="middle" class="tex-formula" src="file://BHXtHcWA.png" style="max-width: 100.0%;max-height: 100.0%;"> integers. <span class="tex-span"><i>i</i></span>-th of them should be equal to maximum length of an odd proper suprefix of <span class="tex-span"><i>i</i></span>-substring of <span class="tex-span"><i>s</i></span> (or <span class="tex-span"> - 1</span>, if there is no such string that is an odd proper suprefix of <span class="tex-span"><i>i</i></span>-substring).</p>





```input1
15
bcabcabcabcabca

```




```input2
24
abaaabaaaabaaabaaaabaaab

```




```input3
19
cabcabbcabcabbcabca

```




```output1
9 7 5 3 1 -1 -1 -1

```




```output2
15 13 11 9 7 5 3 1 1 -1 -1 1

```




```output3
5 3 1 -1 -1 1 1 -1 -1 -1

```



## Note

<p>The answer for first sample test is folowing: </p><ul> <li> 1-substring: <span class="tex-font-style-underline">bcabca<span class="tex-font-style-bf">bca</span></span><span class="tex-font-style-bf">bcabca</span> </li><li> 2-substring: <span class="tex-font-style-underline">cabcab<span class="tex-font-style-bf">c</span></span><span class="tex-font-style-bf">abcabc</span> </li><li> 3-substring: <span class="tex-font-style-underline">abcab</span>c<span class="tex-font-style-bf">abcab</span> </li><li> 4-substring: <span class="tex-font-style-underline">bca</span>bca<span class="tex-font-style-bf">bca</span> </li><li> 5-substring: <span class="tex-font-style-underline">c</span>abcab<span class="tex-font-style-bf">c</span> </li><li> 6-substring: abcab </li><li> 7-substring: bca </li><li> 8-substring: c </li></ul>
