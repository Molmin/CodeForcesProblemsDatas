## Description

<div><p>100 years have passed since the last victory of the man versus computer in Go. Technologies made a huge step forward and robots conquered the Earth! It's time for the final fight between human and robot that will decide the faith of the planet.</p><p>The following game was chosen for the fights: initially there is a polynomial </p><center class="tex-equation"><span class="tex-span"><i>P</i>(<i>x</i>) = <i>a</i><sub class="lower-index"><i>n</i></sub><i>x</i><sup class="upper-index"><i>n</i></sup> + <i>a</i><sub class="lower-index"><i>n</i> - 1</sub><i>x</i><sup class="upper-index"><i>n</i> - 1</sup> + ... + <i>a</i><sub class="lower-index">1</sub><i>x</i> + <i>a</i><sub class="lower-index">0</sub>, </span></center> with yet undefined coefficients and the integer <span class="tex-span"><i>k</i></span>. Players alternate their turns. At each turn, a player pick some index <span class="tex-span"><i>j</i></span>, such that coefficient <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> that stay near <span class="tex-span"><i>x</i><sup class="upper-index"><i>j</i></sup></span> is not determined yet and sets it to <span class="tex-font-style-bf">any</span> value (integer or real, positive or negative, <span class="tex-span">0</span> is also allowed). Computer moves first. The human will be declared the winner if and only if the resulting polynomial will be divisible by <span class="tex-span"><i>Q</i>(<i>x</i>) = <i>x</i> - <i>k</i></span>.<p>Polynomial <span class="tex-span"><i>P</i>(<i>x</i>)</span> is said to be divisible by polynomial <span class="tex-span"><i>Q</i>(<i>x</i>)</span> if there exists a representation <span class="tex-span"><i>P</i>(<i>x</i>) = <i>B</i>(<i>x</i>)<i>Q</i>(<i>x</i>)</span>, where <span class="tex-span"><i>B</i>(<i>x</i>)</span> is also some polynomial.</p><p>Some moves have been made already and now you wonder, is it true that human can guarantee the victory if he plays optimally?</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000, |<i>k</i>| ≤ 10 000</span>)&nbsp;— the size of the polynomial and the integer <span class="tex-span"><i>k</i></span>.</p><p>The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>n</i> + 1</span> lines contain character '<span class="tex-font-style-tt">?</span>' if the coefficient near <span class="tex-span"><i>x</i><sup class="upper-index"><i>i</i> - 1</sup></span> is yet undefined or the integer value <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, if the coefficient is already known (<span class="tex-span"> - 10 000 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10 000</span>). Each of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (and even <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span>) may be equal to <span class="tex-span">0</span>.</p><p>Please note, that it's not guaranteed that you are given the position of the game where it's computer's turn to move.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">Yes</span>" (without quotes) if the human has winning strategy, or "<span class="tex-font-style-tt">No</span>" (without quotes) otherwise.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000, |<i>k</i>| ≤ 10 000</span>)&nbsp;— the size of the polynomial and the integer <span class="tex-span"><i>k</i></span>.</p><p>The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>n</i> + 1</span> lines contain character '<span class="tex-font-style-tt">?</span>' if the coefficient near <span class="tex-span"><i>x</i><sup class="upper-index"><i>i</i> - 1</sup></span> is yet undefined or the integer value <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, if the coefficient is already known (<span class="tex-span"> - 10 000 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10 000</span>). Each of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (and even <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span>) may be equal to <span class="tex-span">0</span>.</p><p>Please note, that it's not guaranteed that you are given the position of the game where it's computer's turn to move.</p>

## Output

<p>Print "<span class="tex-font-style-tt">Yes</span>" (without quotes) if the human has winning strategy, or "<span class="tex-font-style-tt">No</span>" (without quotes) otherwise.</p>





```input1
1 2
-1
?

```




```input2
2 100
-10000
0
1

```




```input3
4 5
?
1
?
1
?

```




```output1
Yes

```




```output2
Yes
```




```output3
No
```



## Note

<p>In the first sample, computer set <span class="tex-span"><i>a</i><sub class="lower-index">0</sub></span> to <span class="tex-span"> - 1</span> on the first move, so if human can set coefficient <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> to <span class="tex-span">0.5</span> and win.</p><p>In the second sample, all coefficients are already set and the resulting polynomial is divisible by <span class="tex-span"><i>x</i> - 100</span>, so the human has won.</p>
