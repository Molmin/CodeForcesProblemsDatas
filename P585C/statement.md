## Description

<div><p>Alice and Bob decided to eat some fruit. In the kitchen they found a large bag of oranges and apples. Alice immediately took an orange for herself, Bob took an apple. To make the process of sharing the remaining fruit more fun, the friends decided to play a game. They put multiple cards and on each one they wrote a letter, either '<span class="tex-font-style-tt">A</span>', or the letter '<span class="tex-font-style-tt">B</span>'. Then they began to remove the cards one by one from left to right, every time they removed a card with the letter '<span class="tex-font-style-tt">A</span>', Alice gave Bob all the fruits she had at that moment and took out of the bag as many apples and as many oranges as she had before. Thus the number of oranges and apples Alice had, did not change. If the card had written letter '<span class="tex-font-style-tt">B</span>', then Bob did the same, that is, he gave Alice all the fruit that he had, and took from the bag the same set of fruit. After the last card way removed, all the fruit in the bag were over.</p><p>You know how many oranges and apples was in the bag at first. Your task is to find any sequence of cards that Alice and Bob could have played with.</p></div><div class="input-specification"><p>The first line of the input contains two integers, <span class="tex-span"><i>x</i>, <i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">18</sup>, <i>xy</i> &gt; 1</span>) — the number of oranges and apples that were initially in the bag.</p></div><div class="output-specification"><p>Print any sequence of cards that would meet the problem conditions as a <span class="tex-font-style-it">compressed</span> string of characters '<span class="tex-font-style-tt">A</span>' and '<span class="tex-font-style-tt">B</span>. That means that you need to replace the segments of identical consecutive characters by the number of repetitions of the characters and the actual character. For example, string <span class="tex-font-style-tt">AAABAABBB</span> should be replaced by string <span class="tex-font-style-tt">3A1B2A3B</span>, but cannot be replaced by <span class="tex-font-style-tt">2A1A1B2A3B</span> or by <span class="tex-font-style-tt">3AB2A3B</span>. See the samples for clarifications of the output format. The string that you print should consist of at most <span class="tex-span">10<sup class="upper-index">6</sup></span> characters. It is guaranteed that if the answer exists, its compressed representation exists, consisting of at most <span class="tex-span">10<sup class="upper-index">6</sup></span> characters. If there are several possible answers, you are allowed to print any of them.</p><p>If the sequence of cards that meet the problem statement does not not exist, print a single word <span class="tex-font-style-tt">Impossible</span>.</p></div>

## Input

<p>The first line of the input contains two integers, <span class="tex-span"><i>x</i>, <i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">18</sup>, <i>xy</i> &gt; 1</span>) — the number of oranges and apples that were initially in the bag.</p>

## Output

<p>Print any sequence of cards that would meet the problem conditions as a <span class="tex-font-style-it">compressed</span> string of characters '<span class="tex-font-style-tt">A</span>' and '<span class="tex-font-style-tt">B</span>. That means that you need to replace the segments of identical consecutive characters by the number of repetitions of the characters and the actual character. For example, string <span class="tex-font-style-tt">AAABAABBB</span> should be replaced by string <span class="tex-font-style-tt">3A1B2A3B</span>, but cannot be replaced by <span class="tex-font-style-tt">2A1A1B2A3B</span> or by <span class="tex-font-style-tt">3AB2A3B</span>. See the samples for clarifications of the output format. The string that you print should consist of at most <span class="tex-span">10<sup class="upper-index">6</sup></span> characters. It is guaranteed that if the answer exists, its compressed representation exists, consisting of at most <span class="tex-span">10<sup class="upper-index">6</sup></span> characters. If there are several possible answers, you are allowed to print any of them.</p><p>If the sequence of cards that meet the problem statement does not not exist, print a single word <span class="tex-font-style-tt">Impossible</span>.</p>





```input1
1 4

```




```input2
2 2

```




```input3
3 2

```




```output1
3B

```




```output2
Impossible

```




```output3
1A1B

```



## Note

<p>In the first sample, if the row contained three cards with letter '<span class="tex-font-style-tt">B</span>', then Bob should give one apple to Alice three times. So, in the end of the game Alice has one orange and three apples, and Bob has one apple, in total it is one orange and four apples.</p><p>In second sample, there is no answer since one card is not enough for game to finish, and two cards will produce at least three apples or three oranges.</p><p>In the third sample, cards contain letters '<span class="tex-font-style-tt">AB</span>', so after removing the first card Bob has one orange and one apple, and after removal of second card Alice has two oranges and one apple. So, in total it is three oranges and two apples.</p>
