## Description

<div><p>You are given string <span class="tex-span"><i>s</i></span> consists of opening and closing brackets of four kinds <span class="tex-font-style-tt">&lt;&gt;</span>, <span class="tex-font-style-tt">{}</span>, <span class="tex-font-style-tt">[]</span>, <span class="tex-font-style-tt">()</span>. There are two types of brackets: opening and closing. You can replace any bracket by another of the same type. For example, you can replace <span class="tex-font-style-tt">&lt;</span> by the bracket <span class="tex-font-style-tt">{</span>, but you can't replace it by <span class="tex-font-style-tt">)</span> or <span class="tex-font-style-tt">&gt;</span>.</p><p>The following definition of a regular bracket sequence is well-known, so you can be familiar with it.</p><p>Let's define a regular bracket sequence (RBS). Empty string is RBS. Let <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> be a RBS then the strings <span class="tex-font-style-tt">&lt;<span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>&gt;<span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span></span>, <span class="tex-font-style-tt">{<span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>}<span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span></span>, <span class="tex-font-style-tt">[<span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>]<span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span></span>, <span class="tex-font-style-tt">(<span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>)<span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span></span> are also RBS.</p><p>For example the string "<span class="tex-font-style-tt">[[(){}]&lt;&gt;]</span>" is RBS, but the strings "<span class="tex-font-style-tt">[)()</span>" and "<span class="tex-font-style-tt">][()()</span>" are not.</p><p>Determine the least number of replaces to make the string <span class="tex-span"><i>s</i></span> RBS.</p></div><div class="input-specification"><p>The only line contains a non empty string <span class="tex-span"><i>s</i></span>, consisting of only opening and closing brackets of four kinds. The length of <span class="tex-span"><i>s</i></span> does not exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p></div><div class="output-specification"><p>If it's impossible to get RBS from <span class="tex-span"><i>s</i></span> print <span class="tex-font-style-tt">Impossible</span>.</p><p>Otherwise print the least number of replaces needed to get RBS from <span class="tex-span"><i>s</i></span>.</p></div>

## Input

<p>The only line contains a non empty string <span class="tex-span"><i>s</i></span>, consisting of only opening and closing brackets of four kinds. The length of <span class="tex-span"><i>s</i></span> does not exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p>

## Output

<p>If it's impossible to get RBS from <span class="tex-span"><i>s</i></span> print <span class="tex-font-style-tt">Impossible</span>.</p><p>Otherwise print the least number of replaces needed to get RBS from <span class="tex-span"><i>s</i></span>.</p>





```input1
[&lt;}){}

```




```input2
{()}[]

```




```input3
]]

```




```output1
2
```




```output2
0
```




```output3
Impossible
```


