## Description

<div><p>Email address in Berland is a string of the form <span class="tex-span"><i>A</i></span>@<span class="tex-span"><i>B</i></span>, where <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> are arbitrary strings consisting of small Latin letters. </p><p>Bob is a system administrator in «Bersoft» company. He keeps a list of email addresses of the company's staff. This list is as a large string, where all addresses are written in arbitrary order, separated by commas. The same address can be written more than once.</p><p>Suddenly, because of unknown reasons, all commas in Bob's list disappeared. Now Bob has a string, where all addresses are written one after another without any separators, and there is impossible to determine, where the boundaries between addresses are. Unfortunately, on the same day his chief asked him to bring the initial list of addresses. Now Bob wants to disjoin addresses in some valid way. Help him to do that.</p></div><div class="input-specification"><p>The first line contains the list of addresses without separators. The length of this string is between <span class="tex-span">1</span> and <span class="tex-span">200</span>, inclusive. The string consists only from small Latin letters and characters «@».</p></div><div class="output-specification"><p>If there is no list of the valid (according to the Berland rules) email addresses such that after removing all commas it coincides with the given string, output <span class="tex-font-style-tt">No solution</span>. In the other case, output the list. The same address can be written in this list more than once. If there are several solutions, output any of them.</p></div>

## Input

<p>The first line contains the list of addresses without separators. The length of this string is between <span class="tex-span">1</span> and <span class="tex-span">200</span>, inclusive. The string consists only from small Latin letters and characters «@».</p>

## Output

<p>If there is no list of the valid (according to the Berland rules) email addresses such that after removing all commas it coincides with the given string, output <span class="tex-font-style-tt">No solution</span>. In the other case, output the list. The same address can be written in this list more than once. If there are several solutions, output any of them.</p>





```input1
a@aa@a

```




```input2
a@a@a

```




```input3
@aa@a

```




```output1
a@a,a@a

```




```output2
No solution

```




```output3
No solution

```


