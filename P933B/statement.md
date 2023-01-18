## Description

<div><p><span class="tex-font-style-it">In order to put away old things and welcome a fresh new year, a thorough cleaning of the house is a must.</span></p><p>Little Tommy finds an old polynomial and cleaned it up by taking it modulo another. But now he regrets doing this...</p><p>Given two integers <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>k</i></span>, find a polynomial <span class="tex-span"><i>f</i>(<i>x</i>)</span> with non-negative integer coefficients strictly less than <span class="tex-span"><i>k</i></span>, whose remainder is <span class="tex-span"><i>p</i></span> when divided by <span class="tex-span">(<i>x</i> + <i>k</i>)</span>. That is, <span class="tex-span"><i>f</i>(<i>x</i>) = <i>q</i>(<i>x</i>)·(<i>x</i> + <i>k</i>) + <i>p</i></span>, where <span class="tex-span"><i>q</i>(<i>x</i>)</span> is a polynomial (not necessarily with integer coefficients).</p></div><div class="input-specification"><p>The only line of input contains two space-separated integers <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>p</i> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span">2 ≤ <i>k</i> ≤ 2 000</span>).</p></div><div class="output-specification"><p>If the polynomial does not exist, print a single integer <span class="tex-font-style-tt">-1</span>, or output two lines otherwise.</p><p>In the first line print a non-negative integer <span class="tex-span"><i>d</i></span> — the number of coefficients in the polynomial.</p><p>In the second line print <span class="tex-span"><i>d</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>d</i> - 1</sub></span>, describing a polynomial <img align="middle" class="tex-formula" src="file://S4ioooZs.png" style="max-width: 100.0%;max-height: 100.0%;"> fulfilling the given requirements. Your output should satisfy <span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>k</i></span> for all <span class="tex-span">0 ≤ <i>i</i> ≤ <i>d</i> - 1</span>, and <span class="tex-span"><i>a</i><sub class="lower-index"><i>d</i> - 1</sub> ≠ 0</span>.</p><p>If there are many possible solutions, print any of them.</p></div>

## Input

<p>The only line of input contains two space-separated integers <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>p</i> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span">2 ≤ <i>k</i> ≤ 2 000</span>).</p>

## Output

<p>If the polynomial does not exist, print a single integer <span class="tex-font-style-tt">-1</span>, or output two lines otherwise.</p><p>In the first line print a non-negative integer <span class="tex-span"><i>d</i></span> — the number of coefficients in the polynomial.</p><p>In the second line print <span class="tex-span"><i>d</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>d</i> - 1</sub></span>, describing a polynomial <img align="middle" class="tex-formula" src="file://S4ioooZs.png" style="max-width: 100.0%;max-height: 100.0%;"> fulfilling the given requirements. Your output should satisfy <span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>k</i></span> for all <span class="tex-span">0 ≤ <i>i</i> ≤ <i>d</i> - 1</span>, and <span class="tex-span"><i>a</i><sub class="lower-index"><i>d</i> - 1</sub> ≠ 0</span>.</p><p>If there are many possible solutions, print any of them.</p>





```input1
46 2

```




```input2
2018 214

```




```output1
7
0 1 0 0 1 1 1

```




```output2
3
92 205 1

```



## Note

<p>In the first example, <span class="tex-span"><i>f</i>(<i>x</i>) = <i>x</i><sup class="upper-index">6</sup> + <i>x</i><sup class="upper-index">5</sup> + <i>x</i><sup class="upper-index">4</sup> + <i>x</i> = (<i>x</i><sup class="upper-index">5</sup> - <i>x</i><sup class="upper-index">4</sup> + 3<i>x</i><sup class="upper-index">3</sup> - 6<i>x</i><sup class="upper-index">2</sup> + 12<i>x</i> - 23)·(<i>x</i> + 2) + 46</span>.</p><p>In the second example, <span class="tex-span"><i>f</i>(<i>x</i>) = <i>x</i><sup class="upper-index">2</sup> + 205<i>x</i> + 92 = (<i>x</i> - 9)·(<i>x</i> + 214) + 2018</span>.</p>
