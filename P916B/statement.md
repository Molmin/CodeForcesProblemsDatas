## Description

<div><p>Jamie is preparing a Codeforces round. He has got an idea for a problem, but does not know how to solve it. Help him write a solution to the following problem:</p><p>Find <span class="tex-span"><i>k</i></span> integers such that the sum of two to the power of each number equals to the number <span class="tex-span"><i>n</i></span> and the largest integer in the answer is as small as possible. As there may be multiple answers, you are asked to output the lexicographically largest one. </p><p>To be more clear, consider all integer sequence with length <span class="tex-span"><i>k</i></span> <span class="tex-span">(<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub>)</span> with <img align="middle" class="tex-formula" src="file://BSSgcb1L.png" style="max-width: 100.0%;max-height: 100.0%;">. Give a value <img align="middle" class="tex-formula" src="file://JpzI379v.png" style="max-width: 100.0%;max-height: 100.0%;"> to each sequence. Among all sequence(s) that have the minimum <span class="tex-span"><i>y</i></span> value, output the one that is the lexicographically largest.</p><p>For definitions of powers and lexicographical order see notes.</p></div><div class="input-specification"><p>The first line consists of two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup>, 1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup>)</span>&nbsp;— the required sum and the length of the sequence.</p></div><div class="output-specification"><p>Output "<span class="tex-font-style-tt">No</span>" (without quotes) in a single line if there does not exist such sequence. Otherwise, output "<span class="tex-font-style-tt">Yes</span>" (without quotes) in the first line, and <span class="tex-span"><i>k</i></span> numbers separated by space in the second line&nbsp;— the required sequence.</p><p>It is guaranteed that the integers in the answer sequence fit the range <span class="tex-span">[ - 10<sup class="upper-index">18</sup>, 10<sup class="upper-index">18</sup>]</span>.</p></div>

## Input

<p>The first line consists of two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup>, 1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup>)</span>&nbsp;— the required sum and the length of the sequence.</p>

## Output

<p>Output "<span class="tex-font-style-tt">No</span>" (without quotes) in a single line if there does not exist such sequence. Otherwise, output "<span class="tex-font-style-tt">Yes</span>" (without quotes) in the first line, and <span class="tex-span"><i>k</i></span> numbers separated by space in the second line&nbsp;— the required sequence.</p><p>It is guaranteed that the integers in the answer sequence fit the range <span class="tex-span">[ - 10<sup class="upper-index">18</sup>, 10<sup class="upper-index">18</sup>]</span>.</p>





```input1
23 5

```




```input2
13 2

```




```input3
1 2

```




```output1
Yes
3 3 2 1 0 

```




```output2
No

```




```output3
Yes
-1 -1 

```



## Note

<p><span class="tex-font-style-bf">Sample 1:</span></p><p><span class="tex-span">2<sup class="upper-index">3</sup> + 2<sup class="upper-index">3</sup> + 2<sup class="upper-index">2</sup> + 2<sup class="upper-index">1</sup> + 2<sup class="upper-index">0</sup> = 8 + 8 + 4 + 2 + 1 = 23</span></p><p>Answers like <span class="tex-span">(3, 3, 2, 0, 1)</span> or <span class="tex-span">(0, 1, 2, 3, 3)</span> are not lexicographically largest.</p><p>Answers like <span class="tex-span">(4, 1, 1, 1, 0)</span> do not have the minimum <span class="tex-span"><i>y</i></span> value.</p><p><span class="tex-font-style-bf">Sample 2:</span></p><p>It can be shown there does not exist a sequence with length 2.</p><p><span class="tex-font-style-bf">Sample 3:</span></p><p><img align="middle" class="tex-formula" src="file://mxp5saQ1.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p><span class="tex-font-style-bf">Powers of 2:</span></p><p>If <span class="tex-span"><i>x</i> &gt; 0</span>, then <span class="tex-span">2<sup class="upper-index"><i>x</i></sup> = 2·2·2·...·2</span> (<span class="tex-span"><i>x</i></span> times).</p><p>If <span class="tex-span"><i>x</i> = 0</span>, then <span class="tex-span">2<sup class="upper-index"><i>x</i></sup> = 1</span>.</p><p>If <span class="tex-span"><i>x</i> &lt; 0</span>, then <img align="middle" class="tex-formula" src="file://YfEuiHAn.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p><span class="tex-font-style-bf">Lexicographical order:</span></p><p>Given two different sequences of the same length, <span class="tex-span">(<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... , <i>a</i><sub class="lower-index"><i>k</i></sub>)</span> and <span class="tex-span">(<i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ... , <i>b</i><sub class="lower-index"><i>k</i></sub>)</span>, the first one is smaller than the second one for the lexicographical order, if and only if <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub></span>, for the first <span class="tex-span"><i>i</i></span> where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> differ.</p>
