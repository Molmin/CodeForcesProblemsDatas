## Description

<div><p>There are three horses living in a horse land: one gray, one white and one gray-and-white. The horses are really amusing animals, which is why they adore special cards. Each of those cards must contain two integers, the first one on top, the second one in the bottom of the card. Let's denote a card with <span class="tex-span"><i>a</i></span> on the top and <span class="tex-span"><i>b</i></span> in the bottom as <span class="tex-span">(<i>a</i>, <i>b</i>)</span>.</p><p>Each of the three horses can paint the special cards. If you show an <span class="tex-span">(<i>a</i>, <i>b</i>)</span> card to the gray horse, then the horse can paint a new <span class="tex-span">(<i>a</i> + 1, <i>b</i> + 1)</span> card. If you show an <span class="tex-span">(<i>a</i>, <i>b</i>)</span> card, such that <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are even integers, to the white horse, then the horse can paint a new <img align="middle" class="tex-formula" src="file://gvNjCrXu.png" style="max-width: 100.0%;max-height: 100.0%;"> card. If you show two cards <span class="tex-span">(<i>a</i>, <i>b</i>)</span> and <span class="tex-span">(<i>b</i>, <i>c</i>)</span> to the gray-and-white horse, then he can paint a new <span class="tex-span">(<i>a</i>, <i>c</i>)</span> card.</p><p>Polycarpus really wants to get <span class="tex-span"><i>n</i></span> special cards <span class="tex-span">(1, <i>a</i><sub class="lower-index">1</sub>)</span>, <span class="tex-span">(1, <i>a</i><sub class="lower-index">2</sub>)</span>, <span class="tex-span">...</span>, <span class="tex-span">(1, <i>a</i><sub class="lower-index"><i>n</i></sub>)</span>. For that he is going to the horse land. He can take exactly one <span class="tex-span">(<i>x</i>, <i>y</i>)</span> card to the horse land, such that <span class="tex-span">1 ≤ <i>x</i> &lt; <i>y</i> ≤ <i>m</i></span>. How many ways are there to choose the card so that he can perform some actions in the horse land and get the required cards?</p><p>Polycarpus can get cards from the horses only as a result of the actions that are described above. Polycarpus is allowed to get additional cards besides the cards that he requires.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 2 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup>)</span>. The second line contains the sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(2 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>. Note, that the numbers in the sequence can coincide.</p><p>The numbers in the lines are separated by single spaces.</p></div><div class="output-specification"><p>Print a single integer — the answer to the problem. </p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in <span class="tex-font-style-it">C++</span>. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 2 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup>)</span>. The second line contains the sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(2 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>. Note, that the numbers in the sequence can coincide.</p><p>The numbers in the lines are separated by single spaces.</p>

## Output

<p>Print a single integer — the answer to the problem. </p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in <span class="tex-font-style-it">C++</span>. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
1 6
2

```




```input2
1 6
7

```




```input3
2 10
13 7

```




```output1
11

```




```output2
14

```




```output3
36

```


