## Description

<div><p>Little penguin Polo loves his home village. The village has <span class="tex-span"><i>n</i></span> houses, indexed by integers from 1 to <span class="tex-span"><i>n</i></span>. Each house has a plaque containing an integer, the <span class="tex-span"><i>i</i></span>-th house has a plaque containing integer <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p><p>Little penguin Polo loves walking around this village. The walk looks like that. First he stands by a house number <span class="tex-span"><i>x</i></span>. Then he goes to the house whose number is written on the plaque of house <span class="tex-span"><i>x</i></span> (that is, to house <span class="tex-span"><i>p</i><sub class="lower-index"><i>x</i></sub></span>), then he goes to the house whose number is written on the plaque of house <span class="tex-span"><i>p</i><sub class="lower-index"><i>x</i></sub></span> (that is, to house <span class="tex-span"><i>p</i><sub class="lower-index"><i>p</i><sub class="lower-index"><i>x</i></sub></sub></span>), and so on.</p><p>We know that:</p><ol> <li> When the penguin starts walking from any house indexed from 1 to <span class="tex-span"><i>k</i></span>, inclusive, he can walk to house number 1. </li><li> When the penguin starts walking from any house indexed from <span class="tex-span"><i>k</i> + 1</span> to <span class="tex-span"><i>n</i></span>, inclusive, he definitely cannot walk to house number 1. </li><li> When the penguin starts walking from house number 1, he can get back to house number 1 after some non-zero number of walks from a house to a house. </li></ol><p>You need to find the number of ways you may write the numbers on the houses' plaques so as to fulfill the three above described conditions. Print the remainder after dividing this number by <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div><div class="input-specification"><p>The single line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000, 1 ≤ <i>k</i> ≤ <i>min</i>(8, <i>n</i>)</span>) — the number of the houses and the number <span class="tex-span"><i>k</i></span> from the statement.</p></div><div class="output-specification"><p>In a single line print a single integer — the answer to the problem modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The single line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000, 1 ≤ <i>k</i> ≤ <i>min</i>(8, <i>n</i>)</span>) — the number of the houses and the number <span class="tex-span"><i>k</i></span> from the statement.</p>

## Output

<p>In a single line print a single integer — the answer to the problem modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
5 2

```




```input2
7 4

```




```output1
54

```




```output2
1728

```


