## Description

<div><p>Little Petya very much likes playing with little Masha. Recently he has received a game called "Zero-One" as a gift from his mother. Petya immediately offered Masha to play the game with him.</p><p>Before the very beginning of the game several cards are lain out on a table in one line from the left to the right. Each card contains a digit: 0 or 1. Players move in turns and Masha moves first. During each move a player should remove a card from the table and shift all other cards so as to close the gap left by the removed card. For example, if before somebody's move the cards on the table formed a sequence 01<span class="tex-font-style-bf">010</span>101, then after the fourth card is removed (the cards are numbered starting from 1), the sequence will look like that: 01<span class="tex-font-style-bf">00</span>101. </p><p>The game ends when exactly two cards are left on the table. The digits on these cards determine the number in binary notation: the most significant bit is located to the left. Masha's aim is to minimize the number and Petya's aim is to maximize it.</p><p>An unpleasant accident occurred before the game started. The kids spilled juice on some of the cards and the digits on the cards got blurred. Each one of the spoiled cards could have either 0 or 1 written on it. Consider all possible variants of initial arrangement of the digits (before the juice spilling). For each variant, let's find which two cards are left by the end of the game, assuming that both Petya and Masha play optimally. An ordered pair of digits written on those two cards is called an <span class="tex-font-style-it">outcome</span>. Your task is to find the set of outcomes for all variants of initial digits arrangement.</p></div><div class="input-specification"><p>The first line contains a sequence of characters each of which can either be a "0", a "1" or a "?". This sequence determines the initial arrangement of cards on the table from the left to the right. The characters "?" mean that the given card was spoiled before the game. The sequence's length ranges from <span class="tex-span">2</span> to <span class="tex-span">10<sup class="upper-index">5</sup></span>, inclusive.</p></div><div class="output-specification"><p>Print the set of outcomes for all possible initial digits arrangements. Print each possible outcome on a single line. Each outcome should be represented by two characters: the digits written on the cards that were left by the end of the game. The outcomes should be sorted lexicographically in ascending order (see the first sample).</p></div>

## Input

<p>The first line contains a sequence of characters each of which can either be a "0", a "1" or a "?". This sequence determines the initial arrangement of cards on the table from the left to the right. The characters "?" mean that the given card was spoiled before the game. The sequence's length ranges from <span class="tex-span">2</span> to <span class="tex-span">10<sup class="upper-index">5</sup></span>, inclusive.</p>

## Output

<p>Print the set of outcomes for all possible initial digits arrangements. Print each possible outcome on a single line. Each outcome should be represented by two characters: the digits written on the cards that were left by the end of the game. The outcomes should be sorted lexicographically in ascending order (see the first sample).</p>





```input1
????

```




```input2
1010

```




```input3
1?1

```




```output1
00
01
10
11

```




```output2
10

```




```output3
01
11

```



## Note

<p>In the first sample all 16 variants of numbers arrangement are possible. For the variant 0000 the outcome is 00. For the variant 1111 the outcome is 11. For the variant 0011 the outcome is 01. For the variant 1100 the outcome is 10. Regardless of outcomes for all other variants the set which we are looking for will contain all 4 possible outcomes.</p><p>In the third sample only 2 variants of numbers arrangement are possible: 111 and 101. For the variant 111 the outcome is 11. For the variant 101 the outcome is 01, because on the first turn Masha can remove the first card from the left after which the game will end.</p>
