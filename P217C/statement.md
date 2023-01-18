## Description

<div><p>The Bytelandian Institute for Biological Research (BIBR) is investigating the properties of two species of bacteria, named simply 0 and 1. Even under a microscope, bacteria of those two species are very difficult to distinguish. In fact, the only thing the scientists possess that is able to differentiate between them is a plant called Formurosa.</p><p>If the scientists place a sample of colonies of bacteria on each on Formurosa's leaves, it will activate a complicated nutrition process. During that process color of Formurosa changes to reflect the result of a — possibly very complicated — logical formula on the species of bacteria, involving constants and the operators <span class="tex-span">|</span> (OR), <span class="tex-span">&amp;</span> (AND) and <span class="tex-span">^</span> (XOR). If it is 0, the plant will turn red, otherwise — it will turn blue.</p><p>For example, if the nutrition process of Formurosa is described by the formula: <span class="tex-span">(((?^?)|?)&amp;(1^?))</span>; then Formurosa has four leaves (the "<span class="tex-font-style-tt">?</span>" signs denote the leaves). If we place <span class="tex-span">0, 1, 0, 0</span> on the respective leaves, the result of the nutrition process will be <span class="tex-span">(((0^1)|0)&amp;(1^0)) = 1</span>, therefore the plant will turn blue.</p><p>The scientists have <span class="tex-span"><i>n</i></span> colonies of bacteria. They do not know their types; the only thing they know for sure is that <span class="tex-font-style-bf">not all colonies are of the same type</span>. They want to attempt to determine the bacteria's species by repeated evaluations with Formurosa. During each evaluation they must place exactly one sample on every leaf of the plant. However, they may use multiple samples of one colony during a single evaluation; they can even cover the whole plant with bacteria from one colony!</p><p>Is it possible for them to always determine the species of each colony, no matter what they are (assuming they are not all the same)?</p></div><div class="input-specification"><p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of colonies of bacteria.</p><p>The second line contains the formula describing the nutrition process of Formurosa. This line contains only characters «<span class="tex-font-style-tt">0</span>», «<span class="tex-font-style-tt">1</span>», «<span class="tex-font-style-tt">?</span>», «<span class="tex-font-style-tt">|</span>», «<span class="tex-font-style-tt">&amp;</span>», «<span class="tex-font-style-tt">^</span>», «<span class="tex-font-style-tt">(</span>», «<span class="tex-font-style-tt">)</span>» and complies with the following grammar:</p><center class="tex-equation"><span class="tex-span"><i>s</i> → 0|1|?|(<i>s</i>|<i>s</i>)|(<i>s</i>&amp;<i>s</i>)|(<i>s</i>^<i>s</i>)</span></center><p>The formula consists of no more than <span class="tex-span">10<sup class="upper-index">6</sup></span> characters.</p></div><div class="output-specification"><p>If it is always possible to determine the species of each colony, output "<span class="tex-font-style-tt">YES</span>" (without quotes). Otherwise, output "<span class="tex-font-style-tt">NO</span>" (without quotes).</p></div>

## Input

<p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of colonies of bacteria.</p><p>The second line contains the formula describing the nutrition process of Formurosa. This line contains only characters «<span class="tex-font-style-tt">0</span>», «<span class="tex-font-style-tt">1</span>», «<span class="tex-font-style-tt">?</span>», «<span class="tex-font-style-tt">|</span>», «<span class="tex-font-style-tt">&amp;</span>», «<span class="tex-font-style-tt">^</span>», «<span class="tex-font-style-tt">(</span>», «<span class="tex-font-style-tt">)</span>» and complies with the following grammar:</p><center class="tex-equation"><span class="tex-span"><i>s</i> → 0|1|?|(<i>s</i>|<i>s</i>)|(<i>s</i>&amp;<i>s</i>)|(<i>s</i>^<i>s</i>)</span></center><p>The formula consists of no more than <span class="tex-span">10<sup class="upper-index">6</sup></span> characters.</p>

## Output

<p>If it is always possible to determine the species of each colony, output "<span class="tex-font-style-tt">YES</span>" (without quotes). Otherwise, output "<span class="tex-font-style-tt">NO</span>" (without quotes).</p>





```input1
2
(?^?)

```




```input2
10
?

```




```input3
2
((?^?)&amp;?)

```




```output1
NO

```




```output2
YES

```




```output3
YES

```


