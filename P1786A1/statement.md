## Description

<div><p><span class="tex-font-style-it">This is an easy version of the problem. In this version, all cards have the same color.</span></p><p>Alice has $n$ cards, each card is white, and the cards are stacked in a deck. Alice deals the cards to herself and to Bob, dealing at once several cards from the top of the deck in the following order: one card to herself, two cards to Bob, three cards to Bob, four cards to herself, five cards to herself, six cards to Bob, seven cards to Bob, eight cards to herself, and so on. In other words, on the $i$-th step, Alice deals $i$ top cards from the deck to one of the players; on the first step, she deals the cards to herself and then alternates the players every two steps. When there aren't enough cards at some step, Alice deals all the remaining cards to the current player, and the process stops.</p><center> <img class="tex-graphics" src="file://bgbKxLMh.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px"> <span class="tex-font-size-small">First Alice's steps in a deck of many cards.</span> </center><p>How many cards will Alice and Bob have at the end?</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 200$). The description of the test cases follows</p><p>The only line of each test case contains a single integer $n$ ($1 \le n \le 10^6$)&nbsp;— the number of cards.</p></div><div class="output-specification"><p>For each test case print two integers&nbsp;— the number of cards in the end for each player&nbsp;— in this order: cards Alice has, cards Bob has.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 200$). The description of the test cases follows</p><p>The only line of each test case contains a single integer $n$ ($1 \le n \le 10^6$)&nbsp;— the number of cards.</p>

## Output

<p>For each test case print two integers&nbsp;— the number of cards in the end for each player&nbsp;— in this order: cards Alice has, cards Bob has.</p>





```input1|2,4,6
5
10
6
17
8
1000000
```




```output1
5 5
1 5
10 7
3 5
500202 499798
```


