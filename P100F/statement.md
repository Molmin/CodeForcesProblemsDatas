## Description

<div><p>You are given a polynom in form <span class="tex-span"><i>p</i>(<i>x</i>) = (<i>x</i> + <i>a</i><sub class="lower-index">1</sub>)·(<i>x</i> + <i>a</i><sub class="lower-index">2</sub>)·... (<i>x</i> + <i>a</i><sub class="lower-index"><i>n</i></sub>)</span>. Write Pike program to print it in a standard form <span class="tex-span"><i>p</i>(<i>x</i>) = <i>x</i><sup class="upper-index"><i>n</i></sup> + <i>b</i><sub class="lower-index">1</sub><i>x</i><sup class="upper-index"><i>n</i> - 1</sup> + ... + <i>b</i><sub class="lower-index"><i>n</i> - 1</sub><i>x</i> + <i>b</i><sub class="lower-index"><i>n</i></sub></span>. You should write each addend in form «<span class="tex-font-style-tt">C*X^K</span>» (for example, <span class="tex-font-style-tt">5*X^8</span>).</p><p>Please, write the polynom in the shortest way, so you should skip unnecessary terms: some terms «<span class="tex-font-style-tt">C*X^K</span>» should be reduced or even omitted. Look for the samples for clarification.</p></div><div class="input-specification"><p>The first line of the input contains <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 9</span>). The following <span class="tex-span"><i>n</i></span> lines contain integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10</span>).</p></div><div class="output-specification"><p>Print the given polynom in a standard way. Note, that the answer in this problem response uniquely determined.</p></div>

## Input

<p>The first line of the input contains <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 9</span>). The following <span class="tex-span"><i>n</i></span> lines contain integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10</span>).</p>

## Output

<p>Print the given polynom in a standard way. Note, that the answer in this problem response uniquely determined.</p>





```input1
2
-1
1

```




```input2
2
1
1

```




```output1
X^2-1

```




```output2
X^2+2*X+1

```


