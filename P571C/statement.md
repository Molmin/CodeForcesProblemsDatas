## Description

<div><p>'In Boolean logic, a formula is in conjunctive normal form (CNF) or clausal normal form if it is a conjunction of clauses, where a clause is a disjunction of literals' (cited from https://en.wikipedia.org/wiki/Conjunctive_normal_form)</p><p>In the other words, CNF is a formula of type <img align="middle" class="tex-formula" src="file://PeFCg1cd.png" style="max-width: 100.0%;max-height: 100.0%;">, where <span class="tex-span">&amp;</span> represents a logical "AND" (conjunction), <img align="middle" class="tex-formula" src="file://P3E8QEOh.png" style="max-width: 100.0%;max-height: 100.0%;"> represents a logical "OR" (disjunction), and <span class="tex-span"><i>v</i><sub class="lower-index"><i>ij</i></sub></span> are some boolean variables or their negations. Each statement in brackets is called a <span class="tex-font-style-it">clause</span>, and <span class="tex-span"><i>v</i><sub class="lower-index"><i>ij</i></sub></span> are called <span class="tex-font-style-it">literals</span>.</p><p>You are given a CNF containing variables <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, ..., <i>x</i><sub class="lower-index"><i>m</i></sub></span> and their negations. We know that each variable occurs in at most two clauses (with negation and without negation in total). Your task is to determine whether this CNF is <span class="tex-font-style-it">satisfiable</span>, that is, whether there are such values of variables where the CNF value is true. If CNF is satisfiable, then you also need to determine the values of the variables at which the CNF is true. </p><p>It is guaranteed that each variable occurs at most once in each clause.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of clauses and the number variables, correspondingly.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain the descriptions of each clause. The <span class="tex-span"><i>i</i></span>-th line first contains first number <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-font-style-bf"><span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub> ≥ 1</span></span>) — the number of literals in the <span class="tex-span"><i>i</i></span>-th clauses. Then follow space-separated literals <span class="tex-span"><i>v</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">1 ≤ |<i>v</i><sub class="lower-index"><i>ij</i></sub>| ≤ <i>m</i></span>). A literal that corresponds to <span class="tex-span"><i>v</i><sub class="lower-index"><i>ij</i></sub></span> is <span class="tex-span"><i>x</i><sub class="lower-index">|<i>v</i><sub class="lower-index"><i>ij</i></sub>|</sub></span> either with negation, if <span class="tex-span"><i>v</i><sub class="lower-index"><i>ij</i></sub></span> is negative, or without negation otherwise.</p></div><div class="output-specification"><p>If CNF is not satisfiable, print a single line "<span class="tex-font-style-tt">NO</span>" (without the quotes), otherwise print two strings: string "<span class="tex-font-style-tt">YES</span>" (without the quotes), and then a string of <span class="tex-span"><i>m</i></span> numbers zero or one — the values of variables in satisfying assignment in the order from <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> to <span class="tex-span"><i>x</i><sub class="lower-index"><i>m</i></sub></span>.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of clauses and the number variables, correspondingly.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain the descriptions of each clause. The <span class="tex-span"><i>i</i></span>-th line first contains first number <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-font-style-bf"><span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub> ≥ 1</span></span>) — the number of literals in the <span class="tex-span"><i>i</i></span>-th clauses. Then follow space-separated literals <span class="tex-span"><i>v</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">1 ≤ |<i>v</i><sub class="lower-index"><i>ij</i></sub>| ≤ <i>m</i></span>). A literal that corresponds to <span class="tex-span"><i>v</i><sub class="lower-index"><i>ij</i></sub></span> is <span class="tex-span"><i>x</i><sub class="lower-index">|<i>v</i><sub class="lower-index"><i>ij</i></sub>|</sub></span> either with negation, if <span class="tex-span"><i>v</i><sub class="lower-index"><i>ij</i></sub></span> is negative, or without negation otherwise.</p>

## Output

<p>If CNF is not satisfiable, print a single line "<span class="tex-font-style-tt">NO</span>" (without the quotes), otherwise print two strings: string "<span class="tex-font-style-tt">YES</span>" (without the quotes), and then a string of <span class="tex-span"><i>m</i></span> numbers zero or one — the values of variables in satisfying assignment in the order from <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> to <span class="tex-span"><i>x</i><sub class="lower-index"><i>m</i></sub></span>.</p>





```input1
2 2
2 1 -2
2 2 -1

```




```input2
4 3
1 1
1 2
3 -1 -2 3
1 -3

```




```input3
5 6
2 1 2
3 1 -2 3
4 -3 5 4 6
2 -6 -4
1 5

```




```output1
YES
11

```




```output2
NO

```




```output3
YES
100010

```



## Note

<p>In the first sample test formula is <img align="middle" class="tex-formula" src="file://mrYoPXPm.png" style="max-width: 100.0%;max-height: 100.0%;">. One of possible answer is <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = <i>TRUE</i>, <i>x</i><sub class="lower-index">2</sub> = <i>TRUE</i></span>.</p>
