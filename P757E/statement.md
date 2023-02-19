## Description

<div><p>Bash got tired on his journey to become the greatest Pokemon master. So he decides to take a break and play with functions.</p><p>Bash defines a function <span class="tex-span"><i>f</i><sub class="lower-index">0</sub>(<i>n</i>)</span>, which denotes the number of ways of factoring <span class="tex-span"><i>n</i></span> into two factors <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span> such that <span class="tex-span"><i>gcd</i>(<i>p</i>, <i>q</i>) = 1</span>. In other words, <span class="tex-span"><i>f</i><sub class="lower-index">0</sub>(<i>n</i>)</span> is the number of ordered pairs of positive integers <span class="tex-span">(<i>p</i>, <i>q</i>)</span> such that <span class="tex-span"><i>p</i>·<i>q</i> = <i>n</i></span> and <span class="tex-span"><i>gcd</i>(<i>p</i>, <i>q</i>) = 1</span>.</p><p>But Bash felt that it was too easy to calculate this function. So he defined a series of functions, where <span class="tex-span"><i>f</i><sub class="lower-index"><i>r</i> + 1</sub></span> is defined as:</p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://Xl6KFGm9.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>Where <span class="tex-span">(<i>u</i>, <i>v</i>)</span> is any ordered pair of positive integers, they need not to be co-prime.</p><p>Now Bash wants to know the value of <span class="tex-span"><i>f</i><sub class="lower-index"><i>r</i></sub>(<i>n</i>)</span> for different <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>n</i></span>. Since the value could be huge, he would like to know the value modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>. Help him!</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the number of values Bash wants to know.</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contain two integers <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>r</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>), which denote Bash wants to know the value <span class="tex-span"><i>f</i><sub class="lower-index"><i>r</i></sub>(<i>n</i>)</span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>q</i></span> integers. For each pair of <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>n</i></span> given, print <span class="tex-span"><i>f</i><sub class="lower-index"><i>r</i></sub>(<i>n</i>)</span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span> on a separate line.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the number of values Bash wants to know.</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contain two integers <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>r</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>), which denote Bash wants to know the value <span class="tex-span"><i>f</i><sub class="lower-index"><i>r</i></sub>(<i>n</i>)</span>.</p>

## Output

<p>Print <span class="tex-span"><i>q</i></span> integers. For each pair of <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>n</i></span> given, print <span class="tex-span"><i>f</i><sub class="lower-index"><i>r</i></sub>(<i>n</i>)</span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span> on a separate line.</p>





```input1
5
0 30
1 25
3 65
2 5
4 48

```




```output1
8
5
25
4
630

```


