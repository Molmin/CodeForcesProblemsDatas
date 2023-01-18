## Description

<div><p>Petya has got <span class="tex-span">2<i>n</i></span> cards, each card contains some integer. The numbers on the cards can be the same. Let's index all cards by consecutive integers from <span class="tex-span">1</span> to <span class="tex-span">2<i>n</i></span>. We'll denote the number that is written on a card with number <span class="tex-span"><i>i</i></span>, as <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. In order to play one entertaining game with his friends, Petya needs to split the cards into pairs so that each pair had equal numbers on the cards. Help Petya do that.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>). The second line contains the sequence of <span class="tex-span">2<i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index">2<i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 5000</span>) — the numbers that are written on the cards. The numbers on the line are separated by single spaces.</p></div><div class="output-specification"><p>If it is impossible to divide the cards into pairs so that cards in each pair had the same numbers, print on a single line integer <span class="tex-font-style-tt">-1</span>. But if the required partition exists, then print <span class="tex-span"><i>n</i></span> pairs of integers, a pair per line — the indices of the cards that form the pairs.</p><p>Separate the numbers on the lines by spaces. You can print the pairs and the numbers in the pairs in any order. If there are multiple solutions, print any of them.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>). The second line contains the sequence of <span class="tex-span">2<i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index">2<i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 5000</span>) — the numbers that are written on the cards. The numbers on the line are separated by single spaces.</p>

## Output

<p>If it is impossible to divide the cards into pairs so that cards in each pair had the same numbers, print on a single line integer <span class="tex-font-style-tt">-1</span>. But if the required partition exists, then print <span class="tex-span"><i>n</i></span> pairs of integers, a pair per line — the indices of the cards that form the pairs.</p><p>Separate the numbers on the lines by spaces. You can print the pairs and the numbers in the pairs in any order. If there are multiple solutions, print any of them.</p>





```input1
3
20 30 10 30 20 10

```




```input2
1
1 2

```




```output1
4 2
1 5
6 3

```




```output2
-1
```


