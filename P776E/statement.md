## Description

<div><p>The Holmes children are fighting over who amongst them is the cleverest.</p><p>Mycroft asked Sherlock and Eurus to find value of <span class="tex-span"><i>f</i>(<i>n</i>)</span>, where <span class="tex-span"><i>f</i>(1) = 1</span> and for <span class="tex-span"><i>n</i> ≥ 2</span>, <span class="tex-span"><i>f</i>(<i>n</i>)</span> is the number of distinct ordered positive integer pairs <span class="tex-span">(<i>x</i>, <i>y</i>)</span> that satisfy <span class="tex-span"><i>x</i> + <i>y</i> = <i>n</i></span> and <span class="tex-span"><i>gcd</i>(<i>x</i>, <i>y</i>) = 1</span>. The integer <span class="tex-span"><i>gcd</i>(<i>a</i>, <i>b</i>)</span> is the greatest common divisor of <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>.</p><p>Sherlock said that solving this was child's play and asked Mycroft to instead get the value of <img align="middle" class="tex-formula" src="file://K1pamj7D.png" style="max-width: 100.0%;max-height: 100.0%;">. Summation is done over all positive integers <span class="tex-span"><i>d</i></span> that divide <span class="tex-span"><i>n</i></span>.</p><p>Eurus was quietly observing all this and finally came up with her problem to astonish both Sherlock and Mycroft.</p><p>She defined a <span class="tex-span"><i>k</i></span>-composite function <span class="tex-span"><i>F</i><sub class="lower-index"><i>k</i></sub>(<i>n</i>)</span> recursively as follows:</p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://ZvsqCWZc.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>She wants them to tell the value of <span class="tex-span"><i>F</i><sub class="lower-index"><i>k</i></sub>(<i>n</i>)</span> modulo <span class="tex-span">1000000007</span>.</p></div><div class="input-specification"><p>A single line of input contains two space separated integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">12</sup></span>) and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">12</sup></span>) indicating that Eurus asks Sherlock and Mycroft to find the value of <span class="tex-span"><i>F</i><sub class="lower-index"><i>k</i></sub>(<i>n</i>)</span> modulo <span class="tex-span">1000000007</span>.</p></div><div class="output-specification"><p>Output a single integer&nbsp;— the value of <span class="tex-span"><i>F</i><sub class="lower-index"><i>k</i></sub>(<i>n</i>)</span> modulo <span class="tex-span">1000000007</span>.</p></div>

## Input

<p>A single line of input contains two space separated integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">12</sup></span>) and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">12</sup></span>) indicating that Eurus asks Sherlock and Mycroft to find the value of <span class="tex-span"><i>F</i><sub class="lower-index"><i>k</i></sub>(<i>n</i>)</span> modulo <span class="tex-span">1000000007</span>.</p>

## Output

<p>Output a single integer&nbsp;— the value of <span class="tex-span"><i>F</i><sub class="lower-index"><i>k</i></sub>(<i>n</i>)</span> modulo <span class="tex-span">1000000007</span>.</p>





```input1
7 1

```




```input2
10 2

```




```output1
6
```




```output2
4
```



## Note

<p>In the first case, there are <span class="tex-span">6</span> distinct ordered pairs <span class="tex-span">(1, 6)</span>, <span class="tex-span">(2, 5)</span>, <span class="tex-span">(3, 4)</span>, <span class="tex-span">(4, 3)</span>, <span class="tex-span">(5, 2)</span> and <span class="tex-span">(6, 1)</span> satisfying <span class="tex-span"><i>x</i> + <i>y</i> = 7</span> and <span class="tex-span"><i>gcd</i>(<i>x</i>, <i>y</i>) = 1</span>. Hence, <span class="tex-span"><i>f</i>(7) = 6</span>. So, <span class="tex-span"><i>F</i><sub class="lower-index">1</sub>(7) = <i>f</i>(<i>g</i>(7)) = <i>f</i>(<i>f</i>(7) + <i>f</i>(1)) = <i>f</i>(6 + 1) = <i>f</i>(7) = 6</span>.</p>
