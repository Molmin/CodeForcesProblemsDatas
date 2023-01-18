## Description

<div><p>Of course, many of you can calculate <span class="tex-span">φ(<i>n</i>)</span> — the number of positive integers that are less than or equal to <span class="tex-span"><i>n</i></span>, that are coprime with <span class="tex-span"><i>n</i></span>. But what if we need to calculate <span class="tex-span">φ(φ(...φ(<i>n</i>)))</span>, where function <span class="tex-span">φ</span> is taken <span class="tex-span"><i>k</i></span> times and <span class="tex-span"><i>n</i></span> is given in the canonical decomposition into prime factors? </p><p>You are given <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span>, calculate the value of <span class="tex-span">φ(φ(...φ(<i>n</i>)))</span>. Print the result in the canonical decomposition into prime factors.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of distinct prime divisors in the canonical representaion of <span class="tex-span"><i>n</i></span>.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains a pair of space-separated integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">2 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>;&nbsp;1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">17</sup></span>) — another prime divisor of number <span class="tex-span"><i>n</i></span> and its power in the canonical representation. The sum of all <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> doesn't exceed <span class="tex-span">10<sup class="upper-index">17</sup></span>. Prime divisors in the input follow in the strictly increasing order.</p><p>The last line contains integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">18</sup></span>).</p></div><div class="output-specification"><p>In the first line, print integer <span class="tex-span"><i>w</i></span> — the number of distinct prime divisors of number <span class="tex-span">φ(φ(...φ(<i>n</i>)))</span>, where function <span class="tex-span">φ</span> is taken <span class="tex-span"><i>k</i></span> times.</p><p>Each of the next <span class="tex-span"><i>w</i></span> lines must contain two space-separated integers <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(<i>b</i><sub class="lower-index"><i>i</i></sub> ≥ 1)</span> — another prime divisor and its power in the canonical representaion of the result. Numbers <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> must go in the strictly increasing order.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of distinct prime divisors in the canonical representaion of <span class="tex-span"><i>n</i></span>.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains a pair of space-separated integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">2 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>;&nbsp;1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">17</sup></span>) — another prime divisor of number <span class="tex-span"><i>n</i></span> and its power in the canonical representation. The sum of all <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> doesn't exceed <span class="tex-span">10<sup class="upper-index">17</sup></span>. Prime divisors in the input follow in the strictly increasing order.</p><p>The last line contains integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">18</sup></span>).</p>

## Output

<p>In the first line, print integer <span class="tex-span"><i>w</i></span> — the number of distinct prime divisors of number <span class="tex-span">φ(φ(...φ(<i>n</i>)))</span>, where function <span class="tex-span">φ</span> is taken <span class="tex-span"><i>k</i></span> times.</p><p>Each of the next <span class="tex-span"><i>w</i></span> lines must contain two space-separated integers <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(<i>b</i><sub class="lower-index"><i>i</i></sub> ≥ 1)</span> — another prime divisor and its power in the canonical representaion of the result. Numbers <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> must go in the strictly increasing order.</p>





```input1
1
7 1
1

```




```input2
1
7 1
2

```




```input3
1
2 100000000000000000
10000000000000000

```




```output1
2
2 1
3 1

```




```output2
1
2 1

```




```output3
1
2 90000000000000000

```



## Note

<p>You can read about canonical representation of a positive integer here: <span class="tex-font-style-tt">http://en.wikipedia.org/wiki/Fundamental_theorem_of_arithmetic</span>.</p><p>You can read about function <span class="tex-span">φ(<i>n</i>)</span> here: <span class="tex-font-style-tt">http://en.wikipedia.org/wiki/Euler's_totient_function</span>.</p>
