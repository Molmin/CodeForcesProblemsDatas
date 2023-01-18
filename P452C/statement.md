## Description

<div><p>Alex enjoys performing magic tricks. He has a trick that requires a deck of <span class="tex-span"><i>n</i></span> cards. He has <span class="tex-span"><i>m</i></span> identical decks of <span class="tex-span"><i>n</i></span> different cards each, which have been mixed together. When Alex wishes to perform the trick, he grabs <span class="tex-span"><i>n</i></span> cards at random and performs the trick with those. The resulting deck looks like a normal deck, but may have duplicates of some cards.</p><p>The trick itself is performed as follows: first Alex allows you to choose a random card from the deck. You memorize the card and put it back in the deck. Then Alex shuffles the deck, and pulls out a card. If the card matches the one you memorized, the trick is successful.</p><p>You don't think Alex is a very good magician, and that he just pulls a card randomly from the deck. Determine the probability of the trick being successful if this is the case.</p></div><div class="input-specification"><p>First line of the input consists of two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>), separated by space — number of cards in each deck, and number of decks.</p></div><div class="output-specification"><p>On the only line of the output print one floating point number – probability of Alex successfully performing the trick. Relative or absolute error of your answer should not be higher than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>First line of the input consists of two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>), separated by space — number of cards in each deck, and number of decks.</p>

## Output

<p>On the only line of the output print one floating point number – probability of Alex successfully performing the trick. Relative or absolute error of your answer should not be higher than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
2 2

```




```input2
4 4

```




```input3
1 2

```




```output1
0.6666666666666666

```




```output2
0.4000000000000000

```




```output3
1.0000000000000000

```



## Note

<p>In the first sample, with probability <img align="middle" class="tex-formula" src="file://X4ePNS2J.png" style="max-width: 100.0%;max-height: 100.0%;"> Alex will perform the trick with two cards with the same value from two different decks. In this case the trick is guaranteed to succeed.</p><p>With the remaining <img align="middle" class="tex-formula" src="file://V6WIneHk.png" style="max-width: 100.0%;max-height: 100.0%;"> probability he took two different cards, and the probability of pulling off the trick is <img align="middle" class="tex-formula" src="file://8OAhkCeO.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>The resulting probability is <img align="middle" class="tex-formula" src="file://2xi6MMoB.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
