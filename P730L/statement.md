## Description

<div><p>A <span class="tex-font-style-it">simplified arithmetic expression</span> (SAE) is an arithmetic expression defined by the following grammar:</p><ul> <li> <span class="tex-font-style-tt">&lt;SAE&gt; ::= &lt;Number&gt; | &lt;SAE&gt;+&lt;SAE&gt; | &lt;SAE&gt;*&lt;SAE&gt; | (&lt;SAE&gt;)</span> </li><li> <span class="tex-font-style-tt">&lt;Number&gt; ::= &lt;Digit&gt; | &lt;Digit&gt;&lt;Number&gt;</span> </li><li> <span class="tex-font-style-tt">&lt;Digit&gt; ::= 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9</span> </li></ul><p>In other words it's a correct arithmetic expression that is allowed to contain brackets, numbers (possibly with leading zeros), multiplications and additions. For example expressions "<span class="tex-font-style-tt">(0+01)</span>", "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">1*(0)</span>" are simplified arithmetic expressions, but expressions "<span class="tex-font-style-tt">2-1</span>", "<span class="tex-font-style-tt">+1</span>" and "<span class="tex-font-style-tt">1+2)</span>" are not.</p><p>Given a string <span class="tex-span"><i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>...<i>s</i><sub class="lower-index">|<i>s</i>|</sub></span> that represents a SAE; <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> denotes the <span class="tex-span"><i>i</i></span>-th character of the string which can be either a digit ('<span class="tex-font-style-tt">0</span>'-'<span class="tex-font-style-tt">9</span>'), a plus sign ('<span class="tex-font-style-tt">+</span>'), a multiplication sign ('<span class="tex-font-style-tt">*</span>'), an opening round bracket '<span class="tex-font-style-tt">(</span>' or a closing round bracket '<span class="tex-font-style-tt">)</span>'.</p><p>A part <span class="tex-span"><i>s</i><sub class="lower-index"><i>l</i></sub><i>s</i><sub class="lower-index"><i>l</i> + 1</sub>...<i>s</i><sub class="lower-index"><i>r</i></sub></span> of this string is called a <span class="tex-font-style-it">sub-expression</span> if and only if it is a SAE.</p><p>You task is to answer <span class="tex-span"><i>m</i></span> queries, each of which is a pair of integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ |<i>s</i>|)</span>. For each query determine whether the corresponding part of the given string is a sub-expression and in case it's a sub-expression calculate its value modulo <span class="tex-span">1000000007&nbsp;(10<sup class="upper-index">9</sup> + 7)</span>. The values should be calculated using standard operator priorities.</p></div><div class="input-specification"><p>The first line of the input contains non-empty string <span class="tex-span"><i>s</i></span> <span class="tex-span">(1 ≤ |<i>s</i>| ≤ 4·10<sup class="upper-index">5</sup>)</span> which represents a correct SAE. Each character of the string can be one of the following characters: '<span class="tex-font-style-tt">*</span>', '<span class="tex-font-style-tt">+</span>', '<span class="tex-font-style-tt">(</span>', '<span class="tex-font-style-tt">)</span>' or a digit ('<span class="tex-font-style-tt">0</span>'-'<span class="tex-font-style-tt">9</span>'). The expression might contain extra-huge numbers.</p><p>The second line contains an integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 4·10<sup class="upper-index">5</sup>)</span> which is the number of queries. Each of the next <span class="tex-span"><i>m</i></span> lines contains two space-separated integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ |<i>s</i>|)</span> — the <span class="tex-span"><i>i</i></span>-th query.</p></div><div class="output-specification"><p>The <span class="tex-span"><i>i</i></span>-th number of output should be the answer for the <span class="tex-span"><i>i</i></span>-th query. If the <span class="tex-span"><i>i</i></span>-th query corresponds to a valid sub-expression output the value of the sub-expression modulo <span class="tex-span">1000000007&nbsp;(10<sup class="upper-index">9</sup> + 7)</span>. Otherwise output -1 as an answer for the query. Print numbers on separate lines.</p></div>

## Input

<p>The first line of the input contains non-empty string <span class="tex-span"><i>s</i></span> <span class="tex-span">(1 ≤ |<i>s</i>| ≤ 4·10<sup class="upper-index">5</sup>)</span> which represents a correct SAE. Each character of the string can be one of the following characters: '<span class="tex-font-style-tt">*</span>', '<span class="tex-font-style-tt">+</span>', '<span class="tex-font-style-tt">(</span>', '<span class="tex-font-style-tt">)</span>' or a digit ('<span class="tex-font-style-tt">0</span>'-'<span class="tex-font-style-tt">9</span>'). The expression might contain extra-huge numbers.</p><p>The second line contains an integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 4·10<sup class="upper-index">5</sup>)</span> which is the number of queries. Each of the next <span class="tex-span"><i>m</i></span> lines contains two space-separated integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ |<i>s</i>|)</span> — the <span class="tex-span"><i>i</i></span>-th query.</p>

## Output

<p>The <span class="tex-span"><i>i</i></span>-th number of output should be the answer for the <span class="tex-span"><i>i</i></span>-th query. If the <span class="tex-span"><i>i</i></span>-th query corresponds to a valid sub-expression output the value of the sub-expression modulo <span class="tex-span">1000000007&nbsp;(10<sup class="upper-index">9</sup> + 7)</span>. Otherwise output -1 as an answer for the query. Print numbers on separate lines.</p>





```input1
((1+2)*3+101*2)
6
8 14
1 6
2 10
11 14
5 5
4 5

```




```input2
(01)
1
1 4

```




```output1
205
-1
10
2
2
-1

```




```output2
1

```


