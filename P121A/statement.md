## Description

<div><p><span class="tex-font-style-underline">Petya loves lucky numbers. Everybody knows that lucky numbers are positive integers whose decimal representation contains only the lucky digits <span class="tex-font-style-bf">4</span> and <span class="tex-font-style-bf">7</span>. For example, numbers <span class="tex-font-style-bf">47</span>, <span class="tex-font-style-bf">744</span>, <span class="tex-font-style-bf">4</span> are lucky and <span class="tex-font-style-bf">5</span>, <span class="tex-font-style-bf">17</span>, <span class="tex-font-style-bf">467</span> are not.</span></p><p>Let <span class="tex-span"><i>next</i>(<i>x</i>)</span> be the minimum lucky number which is larger than or equals <span class="tex-span"><i>x</i></span>. Petya is interested what is the value of the expression <span class="tex-span"><i>next</i>(<i>l</i>) + <i>next</i>(<i>l</i> + 1) + ... + <i>next</i>(<i>r</i> - 1) + <i>next</i>(<i>r</i>)</span>. Help him solve this problem.</p></div><div class="input-specification"><p>The single line contains two integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">9</sup></span>) — the left and right interval limits.</p></div><div class="output-specification"><p>In the single line print the only number — the sum <span class="tex-span"><i>next</i>(<i>l</i>) + <i>next</i>(<i>l</i> + 1) + ... + <i>next</i>(<i>r</i> - 1) + <i>next</i>(<i>r</i>)</span>.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specificator.</p></div>

## Input

<p>The single line contains two integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">9</sup></span>) — the left and right interval limits.</p>

## Output

<p>In the single line print the only number — the sum <span class="tex-span"><i>next</i>(<i>l</i>) + <i>next</i>(<i>l</i> + 1) + ... + <i>next</i>(<i>r</i> - 1) + <i>next</i>(<i>r</i>)</span>.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specificator.</p>





```input1
2 7

```




```input2
7 7

```




```output1
33

```




```output2
7

```



## Note

<p>In the first sample: <span class="tex-span"><i>next</i>(2) + <i>next</i>(3) + <i>next</i>(4) + <i>next</i>(5) + <i>next</i>(6) + <i>next</i>(7) = 4 + 4 + 4 + 7 + 7 + 7 = 33</span></p><p>In the second sample: <span class="tex-span"><i>next</i>(7) = 7</span></p>
