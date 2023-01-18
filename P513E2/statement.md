## Description

<div><p>You are given an array of length <span class="tex-span"><i>n</i></span> and a number <span class="tex-span"><i>k</i></span>. Let's pick <span class="tex-span"><i>k</i></span> non-overlapping non-empty subarrays of the initial array. Let <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> be the sum of the <span class="tex-span"><i>i</i></span>-th subarray in order from left to right. Compute the maximum value of the following expression: </p><center class="tex-equation"><span class="tex-span">|<i>s</i><sub class="lower-index">1</sub> - <i>s</i><sub class="lower-index">2</sub>| + |<i>s</i><sub class="lower-index">2</sub> - <i>s</i><sub class="lower-index">3</sub>| + ... + |<i>s</i><sub class="lower-index"><i>k</i> - 1</sub> - <i>s</i><sub class="lower-index"><i>k</i></sub>|</span></center><p>Here subarray is a contiguous part of an array.</p></div><div class="input-specification"><p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span>. The second line contains <span class="tex-span"><i>n</i></span> integers — the elements of the array. The absolute values of elements do not exceed <span class="tex-span">10<sup class="upper-index">4</sup></span>.</p><p><span class="tex-font-style-it">The problem consists of two subproblems. The subproblems have different constraints on the input. You will get some score for the correct submission of the subproblem. The description of the subproblems follows.</span></p><ul> <li> In subproblem E1 (<span class="tex-span">9</span> points), constraints <span class="tex-span">2 ≤ <i>n</i> ≤ 400</span>, <span class="tex-span">2 ≤ <i>k</i> ≤ <i>min</i>(<i>n</i>, 50)</span> will hold. </li><li> In subproblem E2 (<span class="tex-span">12</span> points), constraints <span class="tex-span">2 ≤ <i>n</i> ≤ 30000</span>, <span class="tex-span">2 ≤ <i>k</i> ≤ <i>min</i>(<i>n</i>, 200)</span> will hold. </li></ul></div><div class="output-specification"><p>Output a single integer — the maximum possible value.</p></div>

## Input

<p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span>. The second line contains <span class="tex-span"><i>n</i></span> integers — the elements of the array. The absolute values of elements do not exceed <span class="tex-span">10<sup class="upper-index">4</sup></span>.</p><p><span class="tex-font-style-it">The problem consists of two subproblems. The subproblems have different constraints on the input. You will get some score for the correct submission of the subproblem. The description of the subproblems follows.</span></p><ul> <li> In subproblem E1 (<span class="tex-span">9</span> points), constraints <span class="tex-span">2 ≤ <i>n</i> ≤ 400</span>, <span class="tex-span">2 ≤ <i>k</i> ≤ <i>min</i>(<i>n</i>, 50)</span> will hold. </li><li> In subproblem E2 (<span class="tex-span">12</span> points), constraints <span class="tex-span">2 ≤ <i>n</i> ≤ 30000</span>, <span class="tex-span">2 ≤ <i>k</i> ≤ <i>min</i>(<i>n</i>, 200)</span> will hold. </li></ul>

## Output

<p>Output a single integer — the maximum possible value.</p>





```input1
5 3
5 2 4 3 1

```




```input2
4 2
7 4 3 7

```




```output1
12

```




```output2
8

```



## Note

<p>Consider the first sample test. The optimal solution is obtained if the first subarray contains the first element only, the second subarray spans the next three elements and the last subarray contains the last element only. The sums of these subarrays are <span class="tex-span">5</span>, <span class="tex-span">9</span> and <span class="tex-span">1</span>, correspondingly.</p><p>Consider the second sample test. In the optimal solution, the first subarray consists of the first two elements and the second subarray consists of the third element only. Note that the last element does not belong to any subarray in this solution.</p>
