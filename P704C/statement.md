## Description

<div><p>Natalia Romanova is trying to test something on the new gun S.H.I.E.L.D gave her. In order to determine the result of the test, she needs to find the number of answers to a certain equation. The equation is of form:</p><p><img align="middle" class="tex-formula" src="file://DEwCcZIo.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Where <img align="middle" class="tex-formula" src="file://dHT34hln.png" style="max-width: 100.0%;max-height: 100.0%;"> represents logical OR and <img align="middle" class="tex-formula" src="file://5BZOHAV9.png" style="max-width: 100.0%;max-height: 100.0%;"> represents logical exclusive OR (XOR), and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> are some boolean variables or their negations. Natalia calls the left side of the equation a XNF formula. Each statement in brackets is called a clause, and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> are called literals.</p><p>In the equation Natalia has, the left side is actually a 2-XNF-2 containing variables <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>m</i></sub></span> and their negations. An XNF formula is 2-XNF-2 if:</p><ol> <li> For each <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>, <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>, i.e. the size of each clause doesn't exceed two. </li><li> Each variable occurs <span class="tex-font-style-bf">in the formula at most two times</span> (with negation and without negation in total). Please note that it's possible that a variable occurs twice but its negation doesn't occur in any clause (or vice versa). </li></ol><p>Natalia is given a formula of <span class="tex-span"><i>m</i></span> variables, consisting of <span class="tex-span"><i>n</i></span> clauses. Please, make sure to check the samples in order to properly understand how the formula looks like.</p><p>Natalia is more into fight than theory, so she asked you to tell her the number of answers to this equation. More precisely, you need to find the number of ways to set <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, ..., <i>x</i><sub class="lower-index"><i>m</i></sub></span> with <span class="tex-span"><i>true</i></span> and <span class="tex-span"><i>false</i></span> (out of total of <span class="tex-span">2<sup class="upper-index"><i>m</i></sup></span> ways) so that the equation is satisfied. Since this number can be extremely large, you need to print the answer modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p><p>Please, note that some variable may appear twice in one clause, or not appear in the equation at all (but still, setting it to <span class="tex-span"><i>false</i></span> or <span class="tex-span"><i>true</i></span> gives different ways to set variables).</p></div><div class="input-specification"><p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100 000</span>)&nbsp;— the number of clauses and the number of variables respectively.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the formula. The <span class="tex-span"><i>i</i></span>-th of them starts with an integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— the number of literals in the <span class="tex-span"><i>i</i></span>-th clause. It is followed by <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> non-zero integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, 1</sub>, ..., <i>a</i><sub class="lower-index"><i>i</i>, <i>k</i><sub class="lower-index"><i>i</i></sub></sub></span>. If <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> &gt; 0</span> then <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> is <span class="tex-span"><i>x</i><sub class="lower-index"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></sub></span> otherwise it's negation of <span class="tex-span"><i>x</i><sub class="lower-index"> - <i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></sub></span> (<span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>, <span class="tex-span"> - <i>m</i> ≤ <i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ <i>m</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≠ 0</span>).</p></div><div class="output-specification"><p>Print the answer modulo <span class="tex-span">1 000 000 007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>) in one line.</p></div>

## Input

<p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100 000</span>)&nbsp;— the number of clauses and the number of variables respectively.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the formula. The <span class="tex-span"><i>i</i></span>-th of them starts with an integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— the number of literals in the <span class="tex-span"><i>i</i></span>-th clause. It is followed by <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> non-zero integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, 1</sub>, ..., <i>a</i><sub class="lower-index"><i>i</i>, <i>k</i><sub class="lower-index"><i>i</i></sub></sub></span>. If <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> &gt; 0</span> then <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> is <span class="tex-span"><i>x</i><sub class="lower-index"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></sub></span> otherwise it's negation of <span class="tex-span"><i>x</i><sub class="lower-index"> - <i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></sub></span> (<span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>, <span class="tex-span"> - <i>m</i> ≤ <i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ <i>m</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≠ 0</span>).</p>

## Output

<p>Print the answer modulo <span class="tex-span">1 000 000 007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>) in one line.</p>





```input1
6 7
2 4 -2
2 6 3
2 -7 1
2 -5 1
2 3 6
2 -2 -5

```




```input2
8 10
1 -5
2 4 -6
2 -2 -6
2 -7 9
2 10 -1
2 3 -1
2 -8 9
2 5 8

```




```input3
2 3
2 1 1
2 -3 3

```




```output1
48

```




```output2
544

```




```output3
4

```



## Note

<p>The equation in the first sample is:</p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://B55wBiRc.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>The equation in the second sample is:</p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://l5rIyQvL.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>The equation in the third sample is:</p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://f65YljcM.png" style="max-width: 100.0%;max-height: 100.0%;"></center>
