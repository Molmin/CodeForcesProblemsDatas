## Description

<div><p>In this problem we consider Boolean functions of four variables <span class="tex-span"><i>A</i>, <i>B</i>, <i>C</i>, <i>D</i></span>. Variables <span class="tex-span"><i>A</i>, <i>B</i>, <i>C</i></span> and <span class="tex-span"><i>D</i></span> are logical and can take values 0 or 1. We will define a function using the following grammar:</p><p><span class="tex-font-style-tt">&lt;expression&gt; ::= &lt;variable&gt; | (&lt;expression&gt;) &lt;operator&gt; (&lt;expression&gt;)</span></p><p><span class="tex-font-style-tt">&lt;variable&gt; ::= 'A' | 'B' | 'C' | 'D' | 'a' | 'b' | 'c' | 'd'</span></p><p><span class="tex-font-style-tt">&lt;operator&gt; ::= '&amp;' | '|'</span></p><p>Here large letters <span class="tex-span"><i>A</i>, <i>B</i>, <i>C</i>, <i>D</i></span> represent variables, and small letters represent their negations. For example, if <span class="tex-span"><i>A</i> = 1</span>, then character <span class="tex-font-style-tt">'A'</span> corresponds to value 1, and value character <span class="tex-font-style-tt">'a'</span> corresponds to value 0. Here character '&amp;' corresponds to the operation of logical AND, character '|' corresponds to the operation of logical OR.</p><p>You are given expression <span class="tex-span"><i>s</i></span>, defining function <span class="tex-span"><i>f</i></span>, where some operations and variables are missing. Also you know the values of the function <span class="tex-span"><i>f</i>(<i>A</i>, <i>B</i>, <i>C</i>, <i>D</i>)</span> for some <span class="tex-span"><i>n</i></span> distinct sets of variable values. Count the number of ways to restore the elements that are missing in the expression so that the resulting expression corresponded to the given information about function <span class="tex-span"><i>f</i></span> in the given variable sets. As the value of the result can be rather large, print its remainder modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line contains expression <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 500</span>), where some characters of the operators and/or variables are replaced by character '?'. </p><p>The second line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 2<sup class="upper-index">4</sup></span>) — the number of integers sets for which we know the value of function <span class="tex-span"><i>f</i>(<i>A</i>, <i>B</i>, <i>C</i>, <i>D</i>)</span>. Next <span class="tex-span"><i>n</i></span> lines contain the descriptions of the sets: the <span class="tex-span"><i>i</i></span>-th of them contains five integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub>, <i>e</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub>, <i>e</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>), separated by spaces and meaning that <span class="tex-span"><i>f</i>(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub>) = <i>e</i><sub class="lower-index"><i>i</i></sub></span>. </p><p>It is guaranteed that all the tuples (<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub></span>) are distinct.</p></div><div class="output-specification"><p>In a single line print the answer to the problem.</p></div>

## Input

<p>The first line contains expression <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 500</span>), where some characters of the operators and/or variables are replaced by character '?'. </p><p>The second line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 2<sup class="upper-index">4</sup></span>) — the number of integers sets for which we know the value of function <span class="tex-span"><i>f</i>(<i>A</i>, <i>B</i>, <i>C</i>, <i>D</i>)</span>. Next <span class="tex-span"><i>n</i></span> lines contain the descriptions of the sets: the <span class="tex-span"><i>i</i></span>-th of them contains five integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub>, <i>e</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub>, <i>e</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>), separated by spaces and meaning that <span class="tex-span"><i>f</i>(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub>) = <i>e</i><sub class="lower-index"><i>i</i></sub></span>. </p><p>It is guaranteed that all the tuples (<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub></span>) are distinct.</p>

## Output

<p>In a single line print the answer to the problem.</p>





```input1
?
2
1 0 1 0 1
0 1 1 0 1

```




```input2
(A)?(?)
1
1 1 0 0 0

```




```input3
((?)&amp;(?))|((?)&amp;(?))
0

```




```input4
b
1
1 0 1 1 1

```




```output1
2

```




```output2
4

```




```output3
4096
```




```output4
1

```



## Note

<p>In the first sample the two valid expressions are 'C' and 'd'.</p><p>In the second sample the expressions look as follows: '(A)&amp;(a)', '(A)&amp;(b)', '(A)&amp;(C)', '(A)&amp;(D)'.</p>
