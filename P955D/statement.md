## Description

<div><p>Jenya has recently acquired quite a useful tool — <span class="tex-span"><i>k</i></span>-scissors for cutting strings. They are generally used for cutting out two non-intersecting substrings of length <span class="tex-span"><i>k</i></span> from an arbitrary string <span class="tex-span"><i>s</i></span> (its length should be at least <span class="tex-span">2·<i>k</i></span> in order to perform this operation) and concatenating them afterwards (preserving the initial order). For example, with the help of <span class="tex-span">2</span>-scissors you can cut <span class="tex-span"><i>ab</i></span> and <span class="tex-span"><i>de</i></span> out of <span class="tex-span"><i>abcde</i></span> and concatenate them into <span class="tex-span"><i>abde</i></span>, but not <span class="tex-span"><i>ab</i></span> and <span class="tex-span"><i>bc</i></span> since they're intersecting.</p><p>It's a nice idea to test this tool before using it in practice. After looking through the papers, Jenya came up with two strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>. His question is whether it is possible to apply his scissors to string <span class="tex-span"><i>s</i></span> such that the resulting concatenation contains <span class="tex-span"><i>t</i></span> as a substring?</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> <span class="tex-span">(2 ≤ <i>m</i> ≤ 2·<i>k</i> ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup>)</span>&nbsp;— length of <span class="tex-span"><i>s</i></span>, length of <span class="tex-span"><i>t</i></span> and the aforementioned scissors' parameter correspondingly.</p><p>The next two lines feature <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> consisting of lowercase latin letters.</p></div><div class="output-specification"><p>If there is no answer, print «<span class="tex-font-style-tt">No</span>». </p><p>Otherwise print «<span class="tex-font-style-tt">Yes</span>» and two integers <span class="tex-span"><i>L</i></span> and <span class="tex-span"><i>R</i></span> denoting the indexes where cutted substrings start (<span class="tex-span">1</span>-indexed). If there are several possible answers, output any.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> <span class="tex-span">(2 ≤ <i>m</i> ≤ 2·<i>k</i> ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup>)</span>&nbsp;— length of <span class="tex-span"><i>s</i></span>, length of <span class="tex-span"><i>t</i></span> and the aforementioned scissors' parameter correspondingly.</p><p>The next two lines feature <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> consisting of lowercase latin letters.</p>

## Output

<p>If there is no answer, print «<span class="tex-font-style-tt">No</span>». </p><p>Otherwise print «<span class="tex-font-style-tt">Yes</span>» and two integers <span class="tex-span"><i>L</i></span> and <span class="tex-span"><i>R</i></span> denoting the indexes where cutted substrings start (<span class="tex-span">1</span>-indexed). If there are several possible answers, output any.</p>





```input1
7 4 3
baabaab
aaaa

```




```input2
6 3 2
cbcbcb
bcc

```




```input3
7 5 3
aabbaaa
aaaaa

```




```output1
Yes
1 5

```




```output2
Yes
2 5

```




```output3
No

```



## Note

<p>In the first sample case you can cut out two substrings starting at <span class="tex-span">1</span> and <span class="tex-span">5</span>. The resulting string <span class="tex-font-style-it">baaaab</span> contains <span class="tex-font-style-it">aaaa</span> as a substring.</p><p>In the second sample case the resulting string is <span class="tex-font-style-it">bccb</span>.</p>
