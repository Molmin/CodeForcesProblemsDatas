## Description

<div><p>You are given an array <span class="tex-span"><i>a</i></span> consisting of <span class="tex-span"><i>n</i></span> positive integers. You pick two integer numbers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, inclusive (numbers are picked randomly, equiprobably and independently). If <span class="tex-span"><i>l</i> &gt; <i>r</i></span>, then you swap values of <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span>. You have to calculate the expected value of the number of unique elements in segment of the array from index <span class="tex-span"><i>l</i></span> to index <span class="tex-span"><i>r</i></span>, inclusive (<span class="tex-span">1</span>-indexed).</p></div><div class="input-specification"><p>The first line contains one integer number <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ... <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span> — elements of the array.</p></div><div class="output-specification"><p>Print one number — the expected number of unique elements in chosen segment. </p><p>Your answer will be considered correct if its absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span> — formally, the answer is correct if <img align="middle" class="tex-formula" src="file://7bdVbxYI.png" style="max-width: 100.0%;max-height: 100.0%;">, where <span class="tex-span"><i>x</i></span> is jury's answer, and <span class="tex-span"><i>y</i></span> is your answer.</p></div>

## Input

<p>The first line contains one integer number <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ... <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span> — elements of the array.</p>

## Output

<p>Print one number — the expected number of unique elements in chosen segment. </p><p>Your answer will be considered correct if its absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span> — formally, the answer is correct if <img align="middle" class="tex-formula" src="file://7bdVbxYI.png" style="max-width: 100.0%;max-height: 100.0%;">, where <span class="tex-span"><i>x</i></span> is jury's answer, and <span class="tex-span"><i>y</i></span> is your answer.</p>





```input1
2
1 2

```




```input2
2
2 2

```




```output1
1.500000

```




```output2
1.000000

```


