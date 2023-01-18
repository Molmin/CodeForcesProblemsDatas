## Description

<div><p><span class="tex-font-style-it">A never-ending, fast-changing and dream-like world unfolds, as the secret door opens.</span></p><p>A <span class="tex-font-style-underline">world</span> is an unordered graph <span class="tex-span"><i>G</i></span>, in whose vertex set <span class="tex-span"><i>V</i>(<i>G</i>)</span> there are two special vertices <span class="tex-span"><i>s</i>(<i>G</i>)</span> and <span class="tex-span"><i>t</i>(<i>G</i>)</span>. An <span class="tex-font-style-underline">initial world</span> has vertex set <span class="tex-span">{<i>s</i>(<i>G</i>), <i>t</i>(<i>G</i>)}</span> and an edge between them.</p><p>A total of <span class="tex-span"><i>n</i></span> changes took place in an <span class="tex-font-style-underline">initial world</span>. In each change, a new vertex <span class="tex-span"><i>w</i></span> is added into <span class="tex-span"><i>V</i>(<i>G</i>)</span>, <span class="tex-font-style-bf">an existing edge</span> <span class="tex-span">(<i>u</i>, <i>v</i>)</span> is chosen, and two edges <span class="tex-span">(<i>u</i>, <i>w</i>)</span> and <span class="tex-span">(<i>v</i>, <i>w</i>)</span> are added into <span class="tex-span"><i>E</i>(<i>G</i>)</span>. Note that it's possible that some edges are chosen in more than one change.</p><p>It's known that the capacity of the minimum <span class="tex-span"><i>s</i></span>-<span class="tex-span"><i>t</i></span> cut of the resulting graph is <span class="tex-span"><i>m</i></span>, that is, at least <span class="tex-span"><i>m</i></span> edges need to be removed in order to make <span class="tex-span"><i>s</i>(<i>G</i>)</span> and <span class="tex-span"><i>t</i>(<i>G</i>)</span> disconnected.</p><p>Count the number of <span class="tex-font-style-it">non-similar worlds</span> that can be built under the constraints, modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>. We define two <span class="tex-font-style-underline">worlds</span> similar, if they are isomorphic and there is isomorphism in which the <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> vertices are not relabelled. Formally, two <span class="tex-font-style-underline">worlds</span> <span class="tex-span"><i>G</i></span> and <span class="tex-span"><i>H</i></span> are considered similar, if there is a bijection between their vertex sets <img align="middle" class="tex-formula" src="file://l1Ua7HIf.png" style="max-width: 100.0%;max-height: 100.0%;">, such that: </p><ul> <li> <span class="tex-span"><i>f</i>(<i>s</i>(<i>G</i>)) = <i>s</i>(<i>H</i>)</span>; </li><li> <span class="tex-span"><i>f</i>(<i>t</i>(<i>G</i>)) = <i>t</i>(<i>H</i>)</span>; </li><li> Two vertices <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> of <span class="tex-span"><i>G</i></span> are adjacent in <span class="tex-span"><i>G</i></span> if and only if <span class="tex-span"><i>f</i>(<i>u</i>)</span> and <span class="tex-span"><i>f</i>(<i>v</i>)</span> are adjacent in <span class="tex-span"><i>H</i></span>. </li></ul></div><div class="input-specification"><p>The first and only line of input contains two space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 50</span>) — the number of operations performed and the minimum cut, respectively.</p></div><div class="output-specification"><p>Output one integer — the number of <span class="tex-font-style-it">non-similar worlds</span> that can be built, modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first and only line of input contains two space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 50</span>) — the number of operations performed and the minimum cut, respectively.</p>

## Output

<p>Output one integer — the number of <span class="tex-font-style-it">non-similar worlds</span> that can be built, modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
3 2

```




```input2
4 4

```




```input3
7 3

```




```input4
31 8

```




```output1
6

```




```output2
3

```




```output3
1196

```




```output4
64921457

```



## Note

<p>In the first example, the following <span class="tex-span">6</span> <span class="tex-font-style-underline">worlds</span> are pairwise non-similar and satisfy the constraints, with <span class="tex-span"><i>s</i>(<i>G</i>)</span> marked in green, <span class="tex-span"><i>t</i>(<i>G</i>)</span> marked in blue, and one of their minimum cuts in light blue.</p><center> <img class="tex-graphics" src="file://8eV9JXTR.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second example, the following <span class="tex-span">3</span> <span class="tex-font-style-underline">worlds</span> satisfy the constraints.</p><center> <img class="tex-graphics" src="file://ApbgzC62.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
