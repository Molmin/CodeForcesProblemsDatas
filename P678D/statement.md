## Description

<div><p>Consider a linear function <span class="tex-span"><i>f</i>(<i>x</i>) = <i>Ax</i> + <i>B</i></span>. Let's define <span class="tex-span"><i>g</i><sup class="upper-index">(0)</sup>(<i>x</i>) = <i>x</i></span> and <span class="tex-span"><i>g</i><sup class="upper-index">(<i>n</i>)</sup>(<i>x</i>) = <i>f</i>(<i>g</i><sup class="upper-index">(<i>n</i> - 1)</sup>(<i>x</i>))</span> for <span class="tex-span"><i>n</i> &gt; 0</span>. For the given integer values <span class="tex-span"><i>A</i></span>, <span class="tex-span"><i>B</i></span>, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>x</i></span> find the value of <span class="tex-span"><i>g</i><sup class="upper-index">(<i>n</i>)</sup>(<i>x</i>)</span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The only line contains four integers <span class="tex-span"><i>A</i></span>, <span class="tex-span"><i>B</i></span>, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>A</i>, <i>B</i>, <i>x</i> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup></span>) — the parameters from the problem statement.</p><p>Note that the given value <span class="tex-span"><i>n</i></span> can be too large, so you should use <span class="tex-span">64</span>-bit integer type to store it. In <span class="tex-font-style-tt">C++</span> you can use the <span class="tex-font-style-tt">long long</span> integer type and in <span class="tex-font-style-tt">Java</span> you can use <span class="tex-font-style-tt">long</span> integer type.</p></div><div class="output-specification"><p>Print the only integer <span class="tex-span"><i>s</i></span> — the value <span class="tex-span"><i>g</i><sup class="upper-index">(<i>n</i>)</sup>(<i>x</i>)</span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The only line contains four integers <span class="tex-span"><i>A</i></span>, <span class="tex-span"><i>B</i></span>, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>A</i>, <i>B</i>, <i>x</i> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup></span>) — the parameters from the problem statement.</p><p>Note that the given value <span class="tex-span"><i>n</i></span> can be too large, so you should use <span class="tex-span">64</span>-bit integer type to store it. In <span class="tex-font-style-tt">C++</span> you can use the <span class="tex-font-style-tt">long long</span> integer type and in <span class="tex-font-style-tt">Java</span> you can use <span class="tex-font-style-tt">long</span> integer type.</p>

## Output

<p>Print the only integer <span class="tex-span"><i>s</i></span> — the value <span class="tex-span"><i>g</i><sup class="upper-index">(<i>n</i>)</sup>(<i>x</i>)</span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
3 4 1 1

```




```input2
3 4 2 1

```




```input3
3 4 3 1

```




```output1
7

```




```output2
25

```




```output3
79

```


