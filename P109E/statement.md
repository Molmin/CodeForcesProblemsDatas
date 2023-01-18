## Description

<div><p><span class="tex-font-style-underline">Petya loves lucky numbers. We all know that lucky numbers are the positive integers whose decimal representations contain only the lucky digits <span class="tex-font-style-bf">4</span> and <span class="tex-font-style-bf">7</span>. For example, numbers <span class="tex-font-style-bf">47</span>, <span class="tex-font-style-bf">744</span>, <span class="tex-font-style-bf">4</span> are lucky and <span class="tex-font-style-bf">5</span>, <span class="tex-font-style-bf">17</span>, <span class="tex-font-style-bf">467</span> are not.</span></p><p>One day Petya came across an interval of numbers <span class="tex-span">[<i>a</i>, <i>a</i> + <i>l</i> - 1]</span>. Let <span class="tex-span"><i>F</i>(<i>x</i>)</span> be the number of lucky digits of number <span class="tex-span"><i>x</i></span>. Find the minimum <span class="tex-span"><i>b</i></span> <span class="tex-span">(<i>a</i> &lt; <i>b</i>)</span> such, that <span class="tex-span"><i>F</i>(<i>a</i>)</span> = <span class="tex-span"><i>F</i>(<i>b</i>)</span>, <span class="tex-span"><i>F</i>(<i>a</i> + 1)</span> = <span class="tex-span"><i>F</i>(<i>b</i> + 1)</span>, ..., <span class="tex-span"><i>F</i>(<i>a</i> + <i>l</i> - 1)</span> = <span class="tex-span"><i>F</i>(<i>b</i> + <i>l</i> - 1)</span>.</p></div><div class="input-specification"><p>The single line contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>l</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>l</i> ≤ 10<sup class="upper-index">9</sup></span>) — the interval's first number and the interval's length correspondingly.</p></div><div class="output-specification"><p>On the single line print number <span class="tex-span"><i>b</i></span> — the answer to the problem.</p></div>

## Input

<p>The single line contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>l</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>l</i> ≤ 10<sup class="upper-index">9</sup></span>) — the interval's first number and the interval's length correspondingly.</p>

## Output

<p>On the single line print number <span class="tex-span"><i>b</i></span> — the answer to the problem.</p>





```input1
7 4

```




```input2
4 7

```




```output1
17

```




```output2
14

```



## Note

<p>Consider that <span class="tex-span">[<i>a</i>, <i>b</i>]</span> denotes an interval of integers; this interval <span class="tex-font-style-bf">includes</span> the boundaries. That is, <img align="middle" class="tex-formula" src="file://2IuaWa0m.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
