## Description

<div><p>Julia is conducting an experiment in her lab. She placed several luminescent bacterial colonies in a horizontal testtube. Different types of bacteria can be distinguished by the color of light they emit. Julia marks types of bacteria with small Latin letters "<span class="tex-font-style-tt">a</span>", ..., "<span class="tex-font-style-tt">z</span>".</p><p>The testtube is divided into <span class="tex-span"><i>n</i></span> consecutive regions. Each region is occupied by a single colony of a certain bacteria type at any given moment. Hence, the population of the testtube at any moment can be described by a string of <span class="tex-span"><i>n</i></span> Latin characters.</p><p>Sometimes a colony can decide to conquer another colony in one of the adjacent regions. When that happens, the attacked colony is immediately eliminated and replaced by a colony of the same type as the attacking colony, while the attacking colony keeps its type. Note that a colony can only attack its neighbours within the boundaries of the testtube. At any moment, at most one attack can take place.</p><p>For example, consider a testtube with population "<span class="tex-font-style-tt">babb</span>". There are six options for an attack that may happen next:</p><ul><li> the first colony attacks the second colony (<span class="tex-span">1 → 2</span>), the resulting population is "<span class="tex-font-style-tt">bbbb</span>";</li><li> <span class="tex-span">2 → 1</span>, the result is "<span class="tex-font-style-tt">aabb</span>";</li><li> <span class="tex-span">2 → 3</span>, the result is "<span class="tex-font-style-tt">baab</span>";</li><li> <span class="tex-span">3 → 2</span>, the result is "<span class="tex-font-style-tt">bbbb</span>" (note that the result is the same as the first option);</li><li> <span class="tex-span">3 → 4</span> or <span class="tex-span">4 → 3</span>, the population does not change.</li></ul><p>The pattern of attacks is rather unpredictable. Julia is now wondering how many different configurations of bacteria in the testtube she can obtain after a sequence of attacks takes place (it is possible that no attacks will happen at all). Since this number can be large, find it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span>&nbsp;— the number of regions in the testtube (<span class="tex-span">1 ≤ <i>n</i> ≤ 5 000</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> small Latin letters that describe the initial population of the testtube.</p></div><div class="output-specification"><p>Print one number&nbsp;— the answer to the problem modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span>&nbsp;— the number of regions in the testtube (<span class="tex-span">1 ≤ <i>n</i> ≤ 5 000</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> small Latin letters that describe the initial population of the testtube.</p>

## Output

<p>Print one number&nbsp;— the answer to the problem modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
3
aaa

```




```input2
2
ab

```




```input3
4
babb

```




```input4
7
abacaba

```




```output1
1

```




```output2
3

```




```output3
11

```




```output4
589

```



## Note

<p>In the first sample the population can never change since all bacteria are of the same type.</p><p>In the second sample three configurations are possible: "<span class="tex-font-style-tt">ab</span>" (no attacks), "<span class="tex-font-style-tt">aa</span>" (the first colony conquers the second colony), and "<span class="tex-font-style-tt">bb</span>" (the second colony conquers the first colony).</p><p>To get the answer for the third sample, note that more than one attack can happen.</p>
