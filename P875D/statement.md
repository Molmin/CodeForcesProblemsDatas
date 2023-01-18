## Description

<div><p><span class="tex-font-style-it">Disclaimer: there are lots of untranslateable puns in the Russian version of the statement, so there is one more reason for you to learn Russian :)</span></p><p>Rick and Morty like to go to the ridge High Cry for crying loudly&nbsp;— there is an extraordinary echo. Recently they discovered an interesting acoustic characteristic of this ridge: if Rick and Morty begin crying simultaneously from different mountains, their cry would be heard between these mountains up to the height equal the bitwise OR of mountains they've climbed and all the mountains between them. </p><p>Bitwise OR is a binary operation which is determined the following way. Consider representation of numbers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> in binary numeric system (probably with leading zeroes) <span class="tex-span"><i>x</i> = <i>x</i><sub class="lower-index"><i>k</i></sub>... <i>x</i><sub class="lower-index">1</sub><i>x</i><sub class="lower-index">0</sub></span> and <span class="tex-span"><i>y</i> = <i>y</i><sub class="lower-index"><i>k</i></sub>... <i>y</i><sub class="lower-index">1</sub><i>y</i><sub class="lower-index">0</sub></span>. Then <span class="tex-span"><i>z</i> = <i>x</i>&nbsp;|&nbsp;<i>y</i></span> is defined following way: <span class="tex-span"><i>z</i> = <i>z</i><sub class="lower-index"><i>k</i></sub>... <i>z</i><sub class="lower-index">1</sub><i>z</i><sub class="lower-index">0</sub></span>, where <span class="tex-span"><i>z</i><sub class="lower-index"><i>i</i></sub> = 1</span>, if <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> = 1</span> or <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub> = 1</span>, and <span class="tex-span"><i>z</i><sub class="lower-index"><i>i</i></sub> = 0</span> otherwise. In the other words, digit of bitwise OR of two numbers equals zero if and only if digits at corresponding positions is both numbers equals zero. For example bitwise OR of numbers <span class="tex-span">10 = 1010<sub class="lower-index">2</sub></span> and <span class="tex-span">9 = 1001<sub class="lower-index">2</sub></span> equals <span class="tex-span">11 = 1011<sub class="lower-index">2</sub></span>. In programming languages C/C++/Java/Python this operation is defined as «<span class="tex-font-style-tt">|</span>», and in Pascal as «<span class="tex-font-style-tt">or</span>».</p><p>Help Rick and Morty calculate the number of ways they can select two mountains in such a way that if they start crying from these mountains their cry will be heard above these mountains and all mountains between them. More formally you should find number of pairs <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> &lt; <i>r</i> ≤ <i>n</i></span>) such that bitwise OR of heights of all mountains between <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (inclusive) is larger than the height of any mountain at this interval.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>), the number of mountains in the ridge.</p><p>Second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), the heights of mountains in order they are located in the ridge.</p></div><div class="output-specification"><p>Print the only integer, the number of ways to choose two different mountains.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>), the number of mountains in the ridge.</p><p>Second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), the heights of mountains in order they are located in the ridge.</p>

## Output

<p>Print the only integer, the number of ways to choose two different mountains.</p>





```input1
5
3 2 1 6 5

```




```input2
4
3 3 3 3

```




```output1
8

```




```output2
0

```



## Note

<p>In the first test case all the ways are pairs of mountains with the numbers (numbering from one):</p><center class="tex-equation"><span class="tex-span">(1, 4), (1, 5), (2, 3), (2, 4), (2, 5), (3, 4), (3, 5), (4, 5)</span></center><p>In the second test case there are no such pairs because for any pair of mountains the height of cry from them is <span class="tex-span">3</span>, and this height is equal to the height of any mountain.</p>
