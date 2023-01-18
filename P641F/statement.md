## Description

<div><p>Little Artem is a very smart programmer. He knows many different difficult algorithms. Recently he has mastered in <span class="tex-font-style-underline">2-SAT</span> one.</p><p>In computer science, 2-satisfiability (abbreviated as <span class="tex-font-style-underline">2-SAT</span>) is the special case of the problem of determining whether a conjunction (logical <span class="tex-font-style-underline">AND</span>) of disjunctions (logical <span class="tex-font-style-underline">OR</span>) have a solution, in which all disjunctions consist of no more than two arguments (variables). For the purpose of this problem we consider only <span class="tex-font-style-underline">2-SAT</span> formulas where each disjunction consists of exactly two arguments.</p><p>Consider the following <span class="tex-font-style-underline">2-SAT</span> problem as an example: <img align="middle" class="tex-formula" src="file://4h3Orm5c.png" style="max-width: 100.0%;max-height: 100.0%;">. Note that there might be negations in <span class="tex-font-style-underline">2-SAT</span> formula (like for <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> and for <span class="tex-span"><i>x</i><sub class="lower-index">4</sub></span>).</p><p>Artem now tries to solve as many problems with <span class="tex-font-style-underline">2-SAT</span> as possible. He found a very interesting one, which he can not solve yet. Of course, he asks you to help him. </p><p>The problem is: given two <span class="tex-font-style-underline">2-SAT</span> formulas <span class="tex-span"><i>f</i></span> and <span class="tex-span"><i>g</i></span>, determine whether their sets of possible solutions are the same. Otherwise, find any variables assignment <span class="tex-span"><i>x</i></span> such that <span class="tex-span"><i>f</i>(<i>x</i>) ≠ <i>g</i>(<i>x</i>)</span>. </p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>m</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>m</i><sub class="lower-index">1</sub>, <i>m</i><sub class="lower-index">2</sub> ≤ <i>n</i><sup class="upper-index">2</sup></span>)&nbsp;— the number of variables, the number of disjunctions in the first formula and the number of disjunctions in the second formula, respectively.</p><p>Next <span class="tex-span"><i>m</i><sub class="lower-index">1</sub></span> lines contains the description of <span class="tex-font-style-underline">2-SAT</span> formula <span class="tex-span"><i>f</i></span>. The description consists of exactly <span class="tex-span"><i>m</i><sub class="lower-index">1</sub></span> pairs of integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - <i>n</i> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>x</i><sub class="lower-index"><i>i</i></sub> ≠ 0</span>) each on separate line, where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> &gt; 0</span> corresponds to the variable without negation, while <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> &lt; 0</span> corresponds to the variable with negation. Each pair gives a single disjunction. Next <span class="tex-span"><i>m</i><sub class="lower-index">2</sub></span> lines contains formula <span class="tex-span"><i>g</i></span> in the similar format.</p></div><div class="output-specification"><p>If both formulas share the same set of solutions, output a single word "<span class="tex-font-style-tt">SIMILAR</span>" (without quotes). Otherwise output exactly <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<img align="middle" class="tex-formula" src="file://tnXdUjx5.png" style="max-width: 100.0%;max-height: 100.0%;">)&nbsp;— any set of values <span class="tex-span"><i>x</i></span> such that <span class="tex-span"><i>f</i>(<i>x</i>) ≠ <i>g</i>(<i>x</i>)</span>.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>m</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>m</i><sub class="lower-index">1</sub>, <i>m</i><sub class="lower-index">2</sub> ≤ <i>n</i><sup class="upper-index">2</sup></span>)&nbsp;— the number of variables, the number of disjunctions in the first formula and the number of disjunctions in the second formula, respectively.</p><p>Next <span class="tex-span"><i>m</i><sub class="lower-index">1</sub></span> lines contains the description of <span class="tex-font-style-underline">2-SAT</span> formula <span class="tex-span"><i>f</i></span>. The description consists of exactly <span class="tex-span"><i>m</i><sub class="lower-index">1</sub></span> pairs of integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - <i>n</i> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>x</i><sub class="lower-index"><i>i</i></sub> ≠ 0</span>) each on separate line, where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> &gt; 0</span> corresponds to the variable without negation, while <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> &lt; 0</span> corresponds to the variable with negation. Each pair gives a single disjunction. Next <span class="tex-span"><i>m</i><sub class="lower-index">2</sub></span> lines contains formula <span class="tex-span"><i>g</i></span> in the similar format.</p>

## Output

<p>If both formulas share the same set of solutions, output a single word "<span class="tex-font-style-tt">SIMILAR</span>" (without quotes). Otherwise output exactly <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<img align="middle" class="tex-formula" src="file://tnXdUjx5.png" style="max-width: 100.0%;max-height: 100.0%;">)&nbsp;— any set of values <span class="tex-span"><i>x</i></span> such that <span class="tex-span"><i>f</i>(<i>x</i>) ≠ <i>g</i>(<i>x</i>)</span>.</p>





```input1
2 1 1
1 2
1 2

```




```input2
2 1 1
1 2
1 -2

```




```output1
SIMILAR

```




```output2
0 0 

```



## Note

<p>First sample has two equal formulas, so they are similar by definition.</p><p>In second sample if we compute first function with <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = 0</span> and <span class="tex-span"><i>x</i><sub class="lower-index">2</sub> = 0</span> we get the result <span class="tex-span">0</span>, because <img align="middle" class="tex-formula" src="file://7IZzDwYG.png" style="max-width: 100.0%;max-height: 100.0%;">. But the second formula is <span class="tex-span">1</span>, because <img align="middle" class="tex-formula" src="file://ZcswjeFS.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
