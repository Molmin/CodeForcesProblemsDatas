## Description

<div><p>Everybody knows what an arithmetic progression is. Let us remind you just in case that an <span class="tex-font-style-it">arithmetic progression</span> is such sequence of numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> of length <span class="tex-span"><i>n</i></span>, that the following condition fulfills: </p><center class="tex-equation"><span class="tex-span"><i>a</i><sub class="lower-index">2</sub> - <i>a</i><sub class="lower-index">1</sub> = <i>a</i><sub class="lower-index">3</sub> - <i>a</i><sub class="lower-index">2</sub> = <i>a</i><sub class="lower-index">4</sub> - <i>a</i><sub class="lower-index">3</sub> = ... = <i>a</i><sub class="lower-index"><i>i</i> + 1</sub> - <i>a</i><sub class="lower-index"><i>i</i></sub> = ... = <i>a</i><sub class="lower-index"><i>n</i></sub> - <i>a</i><sub class="lower-index"><i>n</i> - 1</sub>.</span></center><p>For example, sequences [1, 5], [10], [5, 4, 3] are arithmetic progressions and sequences [1, 3, 2], [1, 2, 4] are not.</p><p>Alexander has <span class="tex-span"><i>n</i></span> cards containing integers. Arthur wants to give Alexander exactly one more card with a number so that he could use the resulting <span class="tex-span"><i>n</i> + 1</span> cards to make an arithmetic progression (Alexander has to use all of his cards).</p><p>Arthur has already bought a card but he hasn't written a number on it. Help him, print all integers that you can write on a card so that the described condition fulfilled.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of cards. The next line contains the sequence of integers — the numbers on Alexander's cards. The numbers are positive integers, each of them doesn't exceed <span class="tex-span">10<sup class="upper-index">8</sup></span>.</p></div><div class="output-specification"><p>If Arthur can write infinitely many distinct integers on the card, print on a single line -1.</p><p>Otherwise, print on the first line the number of integers that suit you. In the second line, print the numbers in the increasing order. Note that the numbers in the answer can exceed <span class="tex-span">10<sup class="upper-index">8</sup></span> or even be negative (see test samples).</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of cards. The next line contains the sequence of integers — the numbers on Alexander's cards. The numbers are positive integers, each of them doesn't exceed <span class="tex-span">10<sup class="upper-index">8</sup></span>.</p>

## Output

<p>If Arthur can write infinitely many distinct integers on the card, print on a single line -1.</p><p>Otherwise, print on the first line the number of integers that suit you. In the second line, print the numbers in the increasing order. Note that the numbers in the answer can exceed <span class="tex-span">10<sup class="upper-index">8</sup></span> or even be negative (see test samples).</p>





```input1
3
4 1 7

```




```input2
1
10

```




```input3
4
1 3 5 9

```




```input4
4
4 3 4 5

```




```input5
2
2 4

```




```output1
2
-2 10

```




```output2
-1

```




```output3
1
7

```




```output4
0

```




```output5
3
0 3 6

```


