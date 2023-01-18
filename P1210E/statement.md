## Description

<div><p>Wojtek has just won a maths competition in Byteland! The prize is admirable — a great book called 'Card Tricks for Everyone.' 'Great!' he thought, 'I can finally use this old, dusted deck of cards that's always been lying unused on my desk!'</p><p>The first chapter of the book is 'How to Shuffle $k$ Cards in Any Order You Want.' It's basically a list of $n$ intricate methods of shuffling the deck of $k$ cards in a deterministic way. Specifically, the $i$-th recipe can be described as a permutation $(P_{i,1}, P_{i,2}, \dots, P_{i,k})$ of integers from $1$ to $k$. If we enumerate the cards in the deck from $1$ to $k$ from top to bottom, then $P_{i,j}$ indicates the number of the $j$-th card from the top of the deck after the shuffle.</p><p>The day is short and Wojtek wants to learn only some of the tricks today. He will pick two integers $l, r$ ($1 \le l \le r \le n$), and he will memorize each trick from the $l$-th to the $r$-th, inclusive. He will then take a sorted deck of $k$ cards and repeatedly apply random memorized tricks until he gets bored. He still likes maths, so he started wondering: how many different decks can he have after he stops shuffling it?</p><p>Wojtek still didn't choose the integers $l$ and $r$, but he is still curious. Therefore, he defined $f(l, r)$ as the number of different decks he can get if he memorizes all the tricks between the $l$-th and the $r$-th, inclusive. What is the value of</p><p>$$\sum_{l=1}^n \sum_{r=l}^n f(l, r)?$$</p></div><div class="input-specification"><p>The first line contains two integers $n$, $k$ ($1 \le n \le 200\,000$, $1 \le k \le 5$) — the number of tricks and the number of cards in Wojtek's deck.</p><p>Each of the following $n$ lines describes a single trick and is described by $k$ distinct integers $P_{i,1}, P_{i,2}, \dots, P_{i, k}$ ($1 \le P_{i, j} \le k$).</p></div><div class="output-specification"><p>Output the value of the sum described in the statement.</p></div>

## Input

<p>The first line contains two integers $n$, $k$ ($1 \le n \le 200\,000$, $1 \le k \le 5$) — the number of tricks and the number of cards in Wojtek's deck.</p><p>Each of the following $n$ lines describes a single trick and is described by $k$ distinct integers $P_{i,1}, P_{i,2}, \dots, P_{i, k}$ ($1 \le P_{i, j} \le k$).</p>

## Output

<p>Output the value of the sum described in the statement.</p>





```input1
3 3
2 1 3
3 1 2
1 3 2
```




```input2
2 4
4 1 3 2
4 3 1 2
```




```output1
25
```




```output2
31
```



## Note

<p>Consider the first sample:</p><ul> <li> The first trick swaps two top cards. </li><li> The second trick takes a card from the bottom and puts it on the top of the deck. </li><li> The third trick swaps two bottom cards. </li></ul><p>The first or the third trick allow Wojtek to generate only two distinct decks (either the two cards are swapped or not). Therefore, $f(1, 1) = f(3, 3) = 2$.</p><p>The second trick allows him to shuffle the deck in a cyclic order. Therefore, $f(2,2)=3$.</p><p>It turns that two first tricks or two last tricks are enough to shuffle the deck in any way desired by Wojtek. Therefore, $f(1,2) = f(2,3) = f(1,3) = 3! = 6$.</p>
