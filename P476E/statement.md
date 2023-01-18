## Description

<div><p>Dreamoon has a string <span class="tex-span"><i>s</i></span> and a pattern string <span class="tex-span"><i>p</i></span>. He first removes exactly <span class="tex-span"><i>x</i></span> characters from <span class="tex-span"><i>s</i></span> obtaining string <span class="tex-span"><i>s</i>'</span> as a result. Then he calculates <img align="middle" class="tex-formula" src="file://FxVGnoRj.png" style="max-width: 100.0%;max-height: 100.0%;"> that is defined as the maximal number of non-overlapping substrings equal to <span class="tex-span"><i>p</i></span> that can be found in <span class="tex-span"><i>s</i>'</span>. He wants to make this number as big as possible.</p><p>More formally, let's define <img align="middle" class="tex-formula" src="file://kvwOzDmF.png" style="max-width: 100.0%;max-height: 100.0%;"> as maximum value of <img align="middle" class="tex-formula" src="file://xLEMi5Qq.png" style="max-width: 100.0%;max-height: 100.0%;"> over all <span class="tex-span"><i>s</i>'</span> that can be obtained by removing exactly <span class="tex-span"><i>x</i></span> characters from <span class="tex-span"><i>s</i></span>. Dreamoon wants to know <img align="middle" class="tex-formula" src="file://kI8bYE71.png" style="max-width: 100.0%;max-height: 100.0%;"> for all <span class="tex-span"><i>x</i></span> from <span class="tex-span">0</span> to <span class="tex-span">|<i>s</i>|</span> where <span class="tex-span">|<i>s</i>|</span> denotes the length of string <span class="tex-span"><i>s</i></span>.</p></div><div class="input-specification"><p>The first line of the input contains the string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 2 000</span>).</p><p>The second line of the input contains the string <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ |<i>p</i>| ≤ 500</span>).</p><p>Both strings will only consist of lower case English letters.</p></div><div class="output-specification"><p>Print <span class="tex-span">|<i>s</i>| + 1</span> space-separated integers in a single line representing the <img align="middle" class="tex-formula" src="file://eKEd2tt7.png" style="max-width: 100.0%;max-height: 100.0%;"> for all <span class="tex-span"><i>x</i></span> from <span class="tex-span">0</span> to <span class="tex-span">|<i>s</i>|</span>.</p></div>

## Input

<p>The first line of the input contains the string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 2 000</span>).</p><p>The second line of the input contains the string <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ |<i>p</i>| ≤ 500</span>).</p><p>Both strings will only consist of lower case English letters.</p>

## Output

<p>Print <span class="tex-span">|<i>s</i>| + 1</span> space-separated integers in a single line representing the <img align="middle" class="tex-formula" src="file://eKEd2tt7.png" style="max-width: 100.0%;max-height: 100.0%;"> for all <span class="tex-span"><i>x</i></span> from <span class="tex-span">0</span> to <span class="tex-span">|<i>s</i>|</span>.</p>





```input1
aaaaa
aa

```




```input2
axbaxxb
ab

```




```output1
2 2 1 1 0 0

```




```output2
0 1 1 2 1 1 0 0

```



## Note

<p>For the first sample, the corresponding optimal values of <span class="tex-span"><i>s</i>'</span> after removal <span class="tex-span">0</span> through <span class="tex-span">|<i>s</i>| = 5</span> characters from <span class="tex-span"><i>s</i></span> are {<span class="tex-font-style-tt">"<span class="tex-font-style-bf">aaaa</span>a"</span>, <span class="tex-font-style-tt">"<span class="tex-font-style-bf">aaaa</span>"</span>, <span class="tex-font-style-tt">"<span class="tex-font-style-bf">aa</span>a"</span>, <span class="tex-font-style-tt">"<span class="tex-font-style-bf">aa</span>"</span>, <span class="tex-font-style-tt">"a"</span>, <span class="tex-font-style-tt">""</span>}. </p><p>For the second sample, possible corresponding optimal values of <span class="tex-span"><i>s</i>'</span> are {<span class="tex-font-style-tt">"axbaxxb"</span>, <span class="tex-font-style-tt">"<span class="tex-font-style-bf">ab</span>axxb"</span>, <span class="tex-font-style-tt">"axb<span class="tex-font-style-bf">ab</span>"</span>, <span class="tex-font-style-tt">"<span class="tex-font-style-bf">abab</span>"</span>, <span class="tex-font-style-tt">"<span class="tex-font-style-bf">ab</span>a"</span>, <span class="tex-font-style-tt">"<span class="tex-font-style-bf">ab</span>"</span>, <span class="tex-font-style-tt">"a"</span>, <span class="tex-font-style-tt">""</span>}.</p>
