## Description

<div><p>Vladik was bored on his way home and decided to play the following game. He took <span class="tex-span"><i>n</i></span> cards and put them in a row in front of himself. Every card has a positive integer number not exceeding <span class="tex-span">8</span> written on it. He decided to find the longest subsequence of cards which satisfies the following conditions:</p><ul> <li> the number of occurrences of each number from <span class="tex-span">1</span> to <span class="tex-span">8</span> in the subsequence doesn't differ by more then <span class="tex-span">1</span> from the number of occurrences of any other number. Formally, if there are <span class="tex-span"><i>c</i><sub class="lower-index"><i>k</i></sub></span> cards with number <span class="tex-span"><i>k</i></span> on them in the subsequence, than for all pairs of integers <img align="middle" class="tex-formula" src="file://bkr3wD1w.png" style="max-width: 100.0%;max-height: 100.0%;"> the condition <span class="tex-span">|<i>c</i><sub class="lower-index"><i>i</i></sub> - <i>c</i><sub class="lower-index"><i>j</i></sub>| ≤ 1</span> must hold. </li><li> if there is at least one card with number <span class="tex-span"><i>x</i></span> on it in the subsequence, then all cards with number <span class="tex-span"><i>x</i></span> in this subsequence must form a continuous segment in it (<span class="tex-font-style-bf">but not necessarily a continuous segment in the original sequence</span>). For example, the subsequence <span class="tex-span">[1, 1, 2, 2]</span> satisfies this condition while the subsequence <span class="tex-span">[1, 2, 2, 1]</span> doesn't. Note that <span class="tex-span">[1, 1, 2, 2]</span> doesn't satisfy the first condition. </li></ul><p>Please help Vladik to find the length of the longest subsequence that satisfies both conditions.</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the number of cards in Vladik's sequence.</p><p>The second line contains the sequence of <span class="tex-span"><i>n</i></span> positive integers not exceeding <span class="tex-span">8</span>&nbsp;— the description of Vladik's sequence.</p></div><div class="output-specification"><p>Print single integer&nbsp;— the length of the longest subsequence of Vladik's sequence that satisfies both conditions.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the number of cards in Vladik's sequence.</p><p>The second line contains the sequence of <span class="tex-span"><i>n</i></span> positive integers not exceeding <span class="tex-span">8</span>&nbsp;— the description of Vladik's sequence.</p>

## Output

<p>Print single integer&nbsp;— the length of the longest subsequence of Vladik's sequence that satisfies both conditions.</p>





```input1
3
1 1 1

```




```input2
8
8 7 6 5 4 3 2 1

```




```input3
24
1 8 1 2 8 2 3 8 3 4 8 4 5 8 5 6 8 6 7 8 7 8 8 8

```




```output1
1
```




```output2
8
```




```output3
17
```



## Note

<p>In the first sample all the numbers written on the cards are equal, so you can't take more than one card, otherwise you'll violate the first condition.</p>
