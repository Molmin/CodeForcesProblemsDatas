## Description

<div><p>Little Johnny has recently learned about set theory. Now he is studying binary relations. You've probably heard the term "equivalence relation". These relations are very important in many areas of mathematics. For example, the equality of the two numbers is an equivalence relation.</p><p>A set <span class="tex-span">ρ</span> of pairs <span class="tex-span">(<i>a</i>, <i>b</i>)</span> of elements of some set <span class="tex-span"><i>A</i></span> is called a binary relation on set <span class="tex-span"><i>A</i></span>. For two elements <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> of the set <span class="tex-span"><i>A</i></span> we say that they are in relation <span class="tex-span">ρ</span>, if pair <img align="middle" class="tex-formula" src="file://iL5PgUzv.png" style="max-width: 100.0%;max-height: 100.0%;">, in this case we use a notation <img align="middle" class="tex-formula" src="file://Eqxo8AKW.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Binary relation is <span class="tex-font-style-it">equivalence relation</span>, if:</p><ol><li> It is reflexive (for any <span class="tex-span"><i>a</i></span> it is true that <img align="middle" class="tex-formula" src="file://INbaYita.png" style="max-width: 100.0%;max-height: 100.0%;">);</li><li> It is symmetric (for any <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> it is true that if <img align="middle" class="tex-formula" src="file://eTH2c9ZK.png" style="max-width: 100.0%;max-height: 100.0%;">, then <img align="middle" class="tex-formula" src="file://v5PDAhUt.png" style="max-width: 100.0%;max-height: 100.0%;">);</li><li> It is transitive (if <img align="middle" class="tex-formula" src="file://NFWPVR1l.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="file://aabvZsva.png" style="max-width: 100.0%;max-height: 100.0%;">, than <img align="middle" class="tex-formula" src="file://j5GEJ52a.png" style="max-width: 100.0%;max-height: 100.0%;">).</li></ol><p>Little Johnny is not completely a fool and he noticed that the first condition is not necessary! Here is his "proof":</p><p>Take any two elements, <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. If <img align="middle" class="tex-formula" src="file://Y4b9InyK.png" style="max-width: 100.0%;max-height: 100.0%;">, then <img align="middle" class="tex-formula" src="file://A6X0n42S.png" style="max-width: 100.0%;max-height: 100.0%;"> (according to property (2)), which means <img align="middle" class="tex-formula" src="file://BqsYaaOh.png" style="max-width: 100.0%;max-height: 100.0%;"> (according to property (3)).</p><p>It's very simple, isn't it? However, you noticed that Johnny's "proof" is wrong, and decided to show him a lot of examples that prove him wrong.</p><p>Here's your task: count the number of binary relations over a set of size <span class="tex-span"><i>n</i></span> such that they are symmetric, transitive, but not an equivalence relations (i.e. they are not reflexive).</p><p>Since their number may be very large (not <span class="tex-span">0</span>, according to Little Johnny), print the remainder of integer division of this number by <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>A single line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 4000)</span>.</p></div><div class="output-specification"><p>In a single line print the answer to the problem modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>A single line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 4000)</span>.</p>

## Output

<p>In a single line print the answer to the problem modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
1

```




```input2
2

```




```input3
3

```




```output1
1

```




```output2
3

```




```output3
10

```



## Note

<p>If <span class="tex-span"><i>n</i> = 1</span> there is only one such relation&nbsp;— an empty one, i.e. <img align="middle" class="tex-formula" src="file://5SR010ox.png" style="max-width: 100.0%;max-height: 100.0%;">. In other words, for a single element <span class="tex-span"><i>x</i></span> of set <span class="tex-span"><i>A</i></span> the following is hold: <img align="middle" class="tex-formula" src="file://QAMYxx75.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>If <span class="tex-span"><i>n</i> = 2</span> there are three such relations. Let's assume that set <span class="tex-span"><i>A</i></span> consists of two elements, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>. Then the valid relations are <img align="middle" class="tex-formula" src="file://JjfQSAnl.png" style="max-width: 100.0%;max-height: 100.0%;">, <span class="tex-span">ρ = {(<i>x</i>, <i>x</i>)}</span>, <span class="tex-span">ρ = {(<i>y</i>, <i>y</i>)}</span>. It is easy to see that the three listed binary relations are symmetric and transitive relations, but they are not equivalence relations.</p>
