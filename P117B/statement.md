## Description

<div><p>In a very ancient country the following game was popular. Two people play the game. Initially first player writes a string <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>, consisting of exactly nine digits and representing a number that does not exceed <span class="tex-span"><i>a</i></span>. After that second player looks at <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and writes a string <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span>, consisting of exactly nine digits and representing a number that does not exceed <span class="tex-span"><i>b</i></span>. Here <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are some given constants, <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> are chosen by the players. The strings are allowed to contain leading zeroes.</p><p>If a number obtained by the concatenation (joining together) of strings <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> is divisible by <span class="tex-span"><i>mod</i></span>, then the second player wins. Otherwise the first player wins. You are given numbers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>mod</i></span>. Your task is to determine who wins if both players play in the optimal manner. If the first player wins, you are also required to find the lexicographically minimum winning move.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>mod</i></span> (<span class="tex-span">0 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>mod</i> ≤ 10<sup class="upper-index">7</sup></span>).</p></div><div class="output-specification"><p>If the first player wins, print "<span class="tex-font-style-tt">1</span>" and the lexicographically minimum string <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> he has to write to win. If the second player wins, print the single number "<span class="tex-font-style-tt">2</span>".</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>mod</i></span> (<span class="tex-span">0 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>mod</i> ≤ 10<sup class="upper-index">7</sup></span>).</p>

## Output

<p>If the first player wins, print "<span class="tex-font-style-tt">1</span>" and the lexicographically minimum string <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> he has to write to win. If the second player wins, print the single number "<span class="tex-font-style-tt">2</span>".</p>





```input1
1 10 7

```




```input2
4 0 9

```




```output1
2

```




```output2
1 000000001

```



## Note

<p>The lexical comparison of strings is performed by the &lt; operator in modern programming languages. String <span class="tex-span"><i>x</i></span> is lexicographically less than string <span class="tex-span"><i>y</i></span> if exists such <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ 9</span>), that <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> &lt; <i>y</i><sub class="lower-index"><i>i</i></sub></span>, and for any <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>j</i> &lt; <i>i</i></span>) <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub> = <i>y</i><sub class="lower-index"><i>j</i></sub></span>. These strings always have length 9.</p>
