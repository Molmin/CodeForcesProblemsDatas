## Description

<div><p>Test data generation is not an easy task! Often, generating big random test cases is not enough to ensure thorough testing of solutions for correctness.</p><p>For example, consider a problem from an old Codeforces round. Its input format looks roughly as follows:</p><p><span class="tex-font-style-it">The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ <i>max</i><sub class="lower-index"><i>n</i></sub></span>)&nbsp;— the size of the set. The second line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>max</i><sub class="lower-index"><i>a</i></sub></span>)&nbsp;— the elements of the set <span class="tex-font-style-bf">in increasing order</span>.</span></p><p>If you don't pay attention to the problem solution, it looks fairly easy to generate a good test case for this problem. Let <span class="tex-span"><i>n</i> = <i>max</i><sub class="lower-index"><i>n</i></sub></span>, take random distinct <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> from 1 to <span class="tex-span"><i>max</i><sub class="lower-index"><i>a</i></sub></span>, sort them... Soon you understand that it's not that easy.</p><p>Here is the actual problem solution. Let <span class="tex-span"><i>g</i></span> be the greatest common divisor of <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. Let <span class="tex-span"><i>x</i> = <i>a</i><sub class="lower-index"><i>n</i></sub> / <i>g</i> - <i>n</i></span>. Then the correct solution outputs "<span class="tex-font-style-tt">Alice</span>" if <span class="tex-span"><i>x</i></span> is odd, and "<span class="tex-font-style-tt">Bob</span>" if <span class="tex-span"><i>x</i></span> is even.</p><p>Consider two wrong solutions to this problem which differ from the correct one only in the formula for calculating <span class="tex-span"><i>x</i></span>.</p><p>The first wrong solution calculates <span class="tex-span"><i>x</i></span> as <span class="tex-span"><i>x</i> = <i>a</i><sub class="lower-index"><i>n</i></sub> / <i>g</i></span> (without subtracting <span class="tex-span"><i>n</i></span>).</p><p>The second wrong solution calculates <span class="tex-span"><i>x</i></span> as <span class="tex-span"><i>x</i> = <i>a</i><sub class="lower-index"><i>n</i></sub> - <i>n</i></span> (without dividing by <span class="tex-span"><i>g</i></span>).</p><p>A test case is interesting if it makes <span class="tex-font-style-bf">both</span> wrong solutions output an incorrect answer.</p><p>Given <span class="tex-span"><i>max</i><sub class="lower-index"><i>n</i></sub></span>, <span class="tex-span"><i>max</i><sub class="lower-index"><i>a</i></sub></span> and <span class="tex-span"><i>q</i></span>, find the number of interesting test cases satisfying the constraints, and output it modulo <span class="tex-span"><i>q</i></span>.</p></div><div class="input-specification"><p>The only line contains three integers <span class="tex-span"><i>max</i><sub class="lower-index"><i>n</i></sub></span>, <span class="tex-span"><i>max</i><sub class="lower-index"><i>a</i></sub></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>max</i><sub class="lower-index"><i>n</i></sub> ≤ 30 000</span>; <span class="tex-span"><i>max</i><sub class="lower-index"><i>n</i></sub> ≤ <i>max</i><sub class="lower-index"><i>a</i></sub> ≤ 10<sup class="upper-index">9</sup></span>; <span class="tex-span">10<sup class="upper-index">4</sup> ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup> + 129</span>).</p></div><div class="output-specification"><p>Output a single integer&nbsp;— the number of test cases which satisfy the constraints and make both wrong solutions output an incorrect answer, modulo <span class="tex-span"><i>q</i></span>.</p></div>

## Input

<p>The only line contains three integers <span class="tex-span"><i>max</i><sub class="lower-index"><i>n</i></sub></span>, <span class="tex-span"><i>max</i><sub class="lower-index"><i>a</i></sub></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>max</i><sub class="lower-index"><i>n</i></sub> ≤ 30 000</span>; <span class="tex-span"><i>max</i><sub class="lower-index"><i>n</i></sub> ≤ <i>max</i><sub class="lower-index"><i>a</i></sub> ≤ 10<sup class="upper-index">9</sup></span>; <span class="tex-span">10<sup class="upper-index">4</sup> ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup> + 129</span>).</p>

## Output

<p>Output a single integer&nbsp;— the number of test cases which satisfy the constraints and make both wrong solutions output an incorrect answer, modulo <span class="tex-span"><i>q</i></span>.</p>





```input1
3 6 100000

```




```input2
6 21 100129

```




```input3
58 787788 50216

```




```output1
4

```




```output2
154

```




```output3
46009

```



## Note

<p>In the first example, interesting test cases look as follows: </p><pre class="verbatim"><br>1              1              1              3<br>2              4              6              2 4 6<br></pre>
