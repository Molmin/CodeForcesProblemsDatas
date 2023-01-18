## Description

<div><p>It is never too late to play the fancy "Binary Cards" game!</p><p>There is an infinite amount of cards of positive and negative ranks that are used in the game. The absolute value of any card rank is a power of two, i.e. each card has a rank of either <span class="tex-span">2<sup class="upper-index"><i>k</i></sup></span> or <span class="tex-span"> - 2<sup class="upper-index"><i>k</i></sup></span> for some integer <span class="tex-span"><i>k</i> ≥ 0</span>. There is an infinite amount of cards of any valid rank.</p><p>At the beginning of the game player forms his deck that is some multiset (possibly empty) of cards. It is allowed to pick any number of cards of any rank but the small deck is considered to be a skill indicator. Game consists of <span class="tex-span"><i>n</i></span> rounds. In the <span class="tex-span"><i>i</i></span>-th round jury tells the player an integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. After that the player is obligated to draw such a subset of his deck that the sum of ranks of the chosen cards is equal to <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (it is allowed to not draw any cards, in which case the sum is considered to be equal to zero). If player fails to do so, he loses and the game is over. Otherwise, player takes back all of his cards into his deck and the game proceeds to the next round. Player is considered a winner if he is able to draw the suitable set of cards in each of the rounds.</p><p>Somebody told you which numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> the jury is going to tell you in each round. Now you want to pick a deck consisting of the minimum number of cards that allows you to win the "Binary Cards" game.</p></div><div class="input-specification"><p>The first line of input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>), the number of rounds in the game.</p><p>The second line of input contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 100 000 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>), the numbers that jury is going to tell in each round.</p></div><div class="output-specification"><p>In the first line print the integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 100 000</span>), the minimum number of cards you have to pick in your deck in ordered to win the "Binary Cards".</p><p>In the second line print <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span"> - 2<sup class="upper-index">20</sup> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 2<sup class="upper-index">20</sup></span>, <span class="tex-span">|<i>b</i><sub class="lower-index"><i>i</i></sub>|</span> is a power of two), the ranks of the cards in your deck. You may output ranks in any order. If there are several optimum decks, you are allowed to print any of them.</p><p>It is guaranteed that there exists a deck of minimum size satisfying all the requirements above.</p></div>

## Input

<p>The first line of input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>), the number of rounds in the game.</p><p>The second line of input contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 100 000 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>), the numbers that jury is going to tell in each round.</p>

## Output

<p>In the first line print the integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 100 000</span>), the minimum number of cards you have to pick in your deck in ordered to win the "Binary Cards".</p><p>In the second line print <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span"> - 2<sup class="upper-index">20</sup> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 2<sup class="upper-index">20</sup></span>, <span class="tex-span">|<i>b</i><sub class="lower-index"><i>i</i></sub>|</span> is a power of two), the ranks of the cards in your deck. You may output ranks in any order. If there are several optimum decks, you are allowed to print any of them.</p><p>It is guaranteed that there exists a deck of minimum size satisfying all the requirements above.</p>





```input1
1
9

```




```input2
5
-1 3 0 4 7

```




```input3
4
2 -2 14 18

```




```output1
2
1 8

```




```output2
3
4 -1 4

```




```output3
3
-2 2 16
```



## Note

<p>In the first sample there is the only round in the game, in which you may simply draw both your cards. Note that this sample test is the only one satisfying the first test group constraints.</p><p>In the second sample you may draw the only card <span class="tex-span"> - 1</span> in the first round, cards <span class="tex-span">4</span> and <span class="tex-span"> - 1</span> in the second round, nothing in the third round, the only card <span class="tex-span">4</span> in the fourth round and the whole deck in the fifth round.</p>
