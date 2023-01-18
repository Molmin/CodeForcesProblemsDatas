## Description

<div><p>You are given two strings <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> consisting of small Latin letters, string <span class="tex-span"><i>s</i></span> can also contain <span class="tex-font-style-tt">'?'</span> characters. </p><p><span class="tex-font-style-it">Suitability</span> of string <span class="tex-span"><i>s</i></span> is calculated by following metric:</p><p>Any two letters can be swapped positions, these operations can be performed arbitrary number of times over any pair of positions. Among all resulting strings <span class="tex-span"><i>s</i></span>, you choose the one with the largest number of <span class="tex-font-style-bf">non-intersecting</span> occurrences of string <span class="tex-span"><i>t</i></span>. <span class="tex-font-style-it">Suitability</span> is this number of occurrences.</p><p>You should replace all <span class="tex-font-style-tt">'?'</span> characters with small Latin letters in such a way that the <span class="tex-font-style-it">suitability</span> of string <span class="tex-span"><i>s</i></span> is maximal.</p></div><div class="input-specification"><p>The first line contains string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">6</sup></span>).</p><p>The second line contains string <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ |<i>t</i>| ≤ 10<sup class="upper-index">6</sup></span>).</p></div><div class="output-specification"><p>Print string <span class="tex-span"><i>s</i></span> with <span class="tex-font-style-tt">'?'</span> replaced with small Latin letters in such a way that <span class="tex-font-style-it">suitability</span> of that string is maximal.</p><p>If there are multiple strings with maximal <span class="tex-font-style-it">suitability</span> then print any of them.</p></div>

## Input

<p>The first line contains string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">6</sup></span>).</p><p>The second line contains string <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ |<i>t</i>| ≤ 10<sup class="upper-index">6</sup></span>).</p>

## Output

<p>Print string <span class="tex-span"><i>s</i></span> with <span class="tex-font-style-tt">'?'</span> replaced with small Latin letters in such a way that <span class="tex-font-style-it">suitability</span> of that string is maximal.</p><p>If there are multiple strings with maximal <span class="tex-font-style-it">suitability</span> then print any of them.</p>





```input1
?aa?
ab

```




```input2
??b?
za

```




```input3
abcd
abacaba

```




```output1
baab

```




```output2
azbz

```




```output3
abcd

```



## Note

<p>In the first example string <span class="tex-font-style-tt">"baab"</span> can be transformed to <span class="tex-font-style-tt">"abab"</span> with swaps, this one has <span class="tex-font-style-it">suitability</span> of <span class="tex-font-style-tt">2</span>. That means that string <span class="tex-font-style-tt">"baab"</span> also has <span class="tex-font-style-it">suitability</span> of <span class="tex-font-style-tt">2</span>.</p><p>In the second example maximal <span class="tex-font-style-it">suitability</span> you can achieve is <span class="tex-font-style-tt">1</span> and there are several dozens of such strings, <span class="tex-font-style-tt">"azbz"</span> is just one of them.</p><p>In the third example there are no <span class="tex-font-style-tt">'?'</span> characters and the <span class="tex-font-style-it">suitability</span> of the string is <span class="tex-font-style-tt">0</span>.</p>
