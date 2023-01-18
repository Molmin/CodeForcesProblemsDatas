## Description

<div><p>You are given a permutation of <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span>. We perform <span class="tex-span"><i>k</i></span> operations of the following type: choose uniformly at random two indices <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span"><i>l</i> ≤ <i>r</i></span>) and reverse the order of the elements <span class="tex-span"><i>p</i><sub class="lower-index"><i>l</i></sub>, <i>p</i><sub class="lower-index"><i>l</i> + 1</sub>, ..., <i>p</i><sub class="lower-index"><i>r</i></sub></span>. Your task is to find the expected value of the number of inversions in the resulting permutation.</p></div><div class="input-specification"><p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>). The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> — the given permutation. All <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> are different and in range from 1 to <span class="tex-span"><i>n</i></span>.</p><p><span class="tex-font-style-it">The problem consists of three subproblems. The subproblems have different constraints on the input. You will get some score for the correct submission of the subproblem. The description of the subproblems follows.</span></p><ul> <li> In subproblem G1 (<span class="tex-span">3</span> points), the constraints <span class="tex-span">1 ≤ <i>n</i> ≤ 6</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 4</span> will hold. </li><li> In subproblem G2 (<span class="tex-span">5</span> points), the constraints <span class="tex-span">1 ≤ <i>n</i> ≤ 30</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 200</span> will hold. </li><li> In subproblem G3 (<span class="tex-span">16</span> points), the constraints <span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span> will hold. </li></ul></div><div class="output-specification"><p>Output the answer with absolute or relative error no more than <span class="tex-span">1<i>e</i> - 9</span>.</p></div>

## Input

<p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>). The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> — the given permutation. All <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> are different and in range from 1 to <span class="tex-span"><i>n</i></span>.</p><p><span class="tex-font-style-it">The problem consists of three subproblems. The subproblems have different constraints on the input. You will get some score for the correct submission of the subproblem. The description of the subproblems follows.</span></p><ul> <li> In subproblem G1 (<span class="tex-span">3</span> points), the constraints <span class="tex-span">1 ≤ <i>n</i> ≤ 6</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 4</span> will hold. </li><li> In subproblem G2 (<span class="tex-span">5</span> points), the constraints <span class="tex-span">1 ≤ <i>n</i> ≤ 30</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 200</span> will hold. </li><li> In subproblem G3 (<span class="tex-span">16</span> points), the constraints <span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span> will hold. </li></ul>

## Output

<p>Output the answer with absolute or relative error no more than <span class="tex-span">1<i>e</i> - 9</span>.</p>





```input1
3 1
1 2 3

```




```input2
3 4
1 3 2

```




```output1
0.833333333333333

```




```output2
1.458333333333334

```



## Note

<p>Consider the first sample test. We will randomly pick an interval of the permutation <span class="tex-span">(1, 2, 3)</span> (which has no inversions) and reverse the order of its elements. With probability <img align="middle" class="tex-formula" src="file://kkLGPZVV.png" style="max-width: 100.0%;max-height: 100.0%;">, the interval will consist of a single element and the permutation will not be altered. With probability <img align="middle" class="tex-formula" src="file://t8RBuuC4.png" style="max-width: 100.0%;max-height: 100.0%;"> we will inverse the first two elements' order and obtain the permutation <span class="tex-span">(2, 1, 3)</span> which has one inversion. With the same probability we might pick the interval consisting of the last two elements which will lead to the permutation <span class="tex-span">(1, 3, 2)</span> with one inversion. Finally, with probability <img align="middle" class="tex-formula" src="file://SxhuYikP.png" style="max-width: 100.0%;max-height: 100.0%;"> the randomly picked interval will contain all elements, leading to the permutation <span class="tex-span">(3, 2, 1)</span> with 3 inversions. Hence, the expected number of inversions is equal to <img align="middle" class="tex-formula" src="file://DIPwvC3t.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
