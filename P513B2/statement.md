## Description

<div><p>You are given a permutation <span class="tex-span"><i>p</i></span> of numbers <span class="tex-span">1, 2, ..., <i>n</i></span>. Let's define <span class="tex-span"><i>f</i>(<i>p</i>)</span> as the following sum:</p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://11Bv66Xi.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>Find the lexicographically <span class="tex-span"><i>m</i></span>-th permutation of length <span class="tex-span"><i>n</i></span> in the set of permutations having the maximum possible value of <span class="tex-span"><i>f</i>(<i>p</i>)</span>.</p></div><div class="input-specification"><p>The single line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>cnt</i><sub class="lower-index"><i>n</i></sub></span>), where <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>n</i></sub></span> is the number of permutations of length <span class="tex-span"><i>n</i></span> with maximum possible value of <span class="tex-span"><i>f</i>(<i>p</i>)</span>.</p><p><span class="tex-font-style-it">The problem consists of two subproblems. The subproblems have different constraints on the input. You will get some score for the correct submission of the subproblem. The description of the subproblems follows.</span></p><ul> <li> In subproblem B1 (<span class="tex-span">3</span> points), the constraint <span class="tex-span">1 ≤ <i>n</i> ≤ 8</span> will hold. </li><li> In subproblem B2 (<span class="tex-span">4</span> points), the constraint <span class="tex-span">1 ≤ <i>n</i> ≤ 50</span> will hold. </li></ul></div><div class="output-specification"><p>Output <span class="tex-span"><i>n</i></span> number forming the required permutation.</p></div>

## Input

<p>The single line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>cnt</i><sub class="lower-index"><i>n</i></sub></span>), where <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>n</i></sub></span> is the number of permutations of length <span class="tex-span"><i>n</i></span> with maximum possible value of <span class="tex-span"><i>f</i>(<i>p</i>)</span>.</p><p><span class="tex-font-style-it">The problem consists of two subproblems. The subproblems have different constraints on the input. You will get some score for the correct submission of the subproblem. The description of the subproblems follows.</span></p><ul> <li> In subproblem B1 (<span class="tex-span">3</span> points), the constraint <span class="tex-span">1 ≤ <i>n</i> ≤ 8</span> will hold. </li><li> In subproblem B2 (<span class="tex-span">4</span> points), the constraint <span class="tex-span">1 ≤ <i>n</i> ≤ 50</span> will hold. </li></ul>

## Output

<p>Output <span class="tex-span"><i>n</i></span> number forming the required permutation.</p>





```input1
2 2

```




```input2
3 2

```




```output1
2 1 

```




```output2
1 3 2 

```



## Note

<p>In the first example, both permutations of numbers {1, 2} yield maximum possible <span class="tex-span"><i>f</i>(<i>p</i>)</span> which is equal to 4. Among them, <span class="tex-span">(2, 1)</span> comes second in lexicographical order.</p>
