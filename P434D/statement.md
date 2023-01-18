## Description

<div><p>Nanami likes playing games, and is also really good at it. This day she was playing a new game which involved operating a power plant. Nanami's job is to control the generators in the plant and produce maximum output.</p><p>There are <span class="tex-span"><i>n</i></span> generators in the plant. Each generator should be set to a generating level. Generating level is an integer (possibly zero or negative), the generating level of the <span class="tex-span"><i>i</i></span>-th generator should be between <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (both inclusive). The output of a generator can be calculated using a certain quadratic function <span class="tex-span"><i>f</i>(<i>x</i>)</span>, where <span class="tex-span"><i>x</i></span> is the generating level of the generator. Each generator has its own function, the function of the <span class="tex-span"><i>i</i></span>-th generator is denoted as <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub>(<i>x</i>)</span>.</p><p>However, there are <span class="tex-span"><i>m</i></span> further restrictions to the generators. Let the generating level of the <span class="tex-span"><i>i</i></span>-th generator be <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>. Each restriction is of the form <span class="tex-span"><i>x</i><sub class="lower-index"><i>u</i></sub> ≤ <i>x</i><sub class="lower-index"><i>v</i></sub> + <i>d</i></span>, where <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> are IDs of two different generators and <span class="tex-span"><i>d</i></span> is an integer.</p><p>Nanami found the game tedious but giving up is against her creed. So she decided to have a program written to calculate the answer for her (the maximum total output of generators). Somehow, this became your job.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i>&nbsp;(1 ≤ <i>n</i> ≤ 50;&nbsp;0 ≤ <i>m</i> ≤ 100)</span> — the number of generators and the number of restrictions.</p><p>Then follow <span class="tex-span"><i>n</i></span> lines, each line contains three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub>&nbsp;(|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 10;&nbsp;|<i>b</i><sub class="lower-index"><i>i</i></sub>|, |<i>c</i><sub class="lower-index"><i>i</i></sub>| ≤ 1000)</span> — the coefficients of the function <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub>(<i>x</i>)</span>. That is, <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub>(<i>x</i>) = <i>a</i><sub class="lower-index"><i>i</i></sub><i>x</i><sup class="upper-index">2</sup> + <i>b</i><sub class="lower-index"><i>i</i></sub><i>x</i> + <i>c</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Then follow another <span class="tex-span"><i>n</i></span> lines, each line contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub>&nbsp;( - 100 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span>.</p><p>Then follow <span class="tex-span"><i>m</i></span> lines, each line contains three integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, and <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub>&nbsp;(1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub>;&nbsp;|<i>d</i><sub class="lower-index"><i>i</i></sub>| ≤ 200)</span>, describing a restriction. The <span class="tex-span"><i>i</i></span>-th restriction is <span class="tex-span"><i>x</i><sub class="lower-index"><i>u</i><sub class="lower-index"><i>i</i></sub></sub> ≤ <i>x</i><sub class="lower-index"><i>v</i><sub class="lower-index"><i>i</i></sub></sub> + <i>d</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="output-specification"><p>Print a single line containing a single integer — the maximum output of all the generators. It is guaranteed that there exists at least one valid configuration.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i>&nbsp;(1 ≤ <i>n</i> ≤ 50;&nbsp;0 ≤ <i>m</i> ≤ 100)</span> — the number of generators and the number of restrictions.</p><p>Then follow <span class="tex-span"><i>n</i></span> lines, each line contains three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub>&nbsp;(|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 10;&nbsp;|<i>b</i><sub class="lower-index"><i>i</i></sub>|, |<i>c</i><sub class="lower-index"><i>i</i></sub>| ≤ 1000)</span> — the coefficients of the function <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub>(<i>x</i>)</span>. That is, <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub>(<i>x</i>) = <i>a</i><sub class="lower-index"><i>i</i></sub><i>x</i><sup class="upper-index">2</sup> + <i>b</i><sub class="lower-index"><i>i</i></sub><i>x</i> + <i>c</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Then follow another <span class="tex-span"><i>n</i></span> lines, each line contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub>&nbsp;( - 100 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span>.</p><p>Then follow <span class="tex-span"><i>m</i></span> lines, each line contains three integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, and <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub>&nbsp;(1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub>;&nbsp;|<i>d</i><sub class="lower-index"><i>i</i></sub>| ≤ 200)</span>, describing a restriction. The <span class="tex-span"><i>i</i></span>-th restriction is <span class="tex-span"><i>x</i><sub class="lower-index"><i>u</i><sub class="lower-index"><i>i</i></sub></sub> ≤ <i>x</i><sub class="lower-index"><i>v</i><sub class="lower-index"><i>i</i></sub></sub> + <i>d</i><sub class="lower-index"><i>i</i></sub></span>.</p>

## Output

<p>Print a single line containing a single integer — the maximum output of all the generators. It is guaranteed that there exists at least one valid configuration.</p>





```input1
3 3
0 1 0
0 1 1
0 1 2
0 3
1 2
-100 100
1 2 0
2 3 0
3 1 0

```




```input2
5 8
1 -8 20
2 -4 0
-1 10 -10
0 1 0
0 -1 1
1 9
1 4
0 10
3 11
7 9
2 1 3
1 2 3
2 3 3
3 2 3
3 4 3
4 3 3
4 5 3
5 4 3

```




```output1
9

```




```output2
46

```



## Note

<p>In the first sample, <span class="tex-span"><i>f</i><sub class="lower-index">1</sub>(<i>x</i>) = <i>x</i></span>, <span class="tex-span"><i>f</i><sub class="lower-index">2</sub>(<i>x</i>) = <i>x</i> + 1</span>, and <span class="tex-span"><i>f</i><sub class="lower-index">3</sub>(<i>x</i>) = <i>x</i> + 2</span>, so we are to maximize the sum of the generating levels. The restrictions are <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub> ≤ <i>x</i><sub class="lower-index">3</sub></span>, and <span class="tex-span"><i>x</i><sub class="lower-index">3</sub> ≤ <i>x</i><sub class="lower-index">1</sub></span>, which gives us <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = <i>x</i><sub class="lower-index">2</sub> = <i>x</i><sub class="lower-index">3</sub></span>. The optimal configuration is <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = <i>x</i><sub class="lower-index">2</sub> = <i>x</i><sub class="lower-index">3</sub> = 2</span>, which produces an output of 9.</p><p>In the second sample, restrictions are equal to <span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub> - <i>x</i><sub class="lower-index"><i>i</i> + 1</sub>| ≤ 3</span> for <span class="tex-span">1 ≤ <i>i</i> &lt; <i>n</i></span>. One of the optimal configurations is <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = 1</span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub> = 4</span>, <span class="tex-span"><i>x</i><sub class="lower-index">3</sub> = 5</span>, <span class="tex-span"><i>x</i><sub class="lower-index">4</sub> = 8</span> and <span class="tex-span"><i>x</i><sub class="lower-index">5</sub> = 7</span>.</p>
