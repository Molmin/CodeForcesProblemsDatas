## Description

<div><p>Have you ever played Hanabi? If not, then you've got to try it out! This problem deals with a simplified version of the game.</p><p>Overall, the game has 25 types of cards (5 distinct colors and 5 distinct values). Borya is holding <span class="tex-span"><i>n</i></span> cards. The game is somewhat complicated by the fact that everybody sees Borya's cards except for Borya himself. Borya knows which cards he has but he knows nothing about the order they lie in. Note that Borya can have multiple identical cards (and for each of the 25 types of cards he knows exactly how many cards of this type he has).</p><p>The aim of the other players is to achieve the state when Borya knows the color and number value of each of his cards. For that, other players can give him hints. The hints can be of two types: color hints and value hints. </p><p>A color hint goes like that: a player names some color and points at all the cards of this color. </p><p>Similarly goes the value hint. A player names some value and points at all the cards that contain the value.</p><p>Determine what minimum number of hints the other players should make for Borya to be certain about each card's color and value.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of Borya's cards. The next line contains the descriptions of <span class="tex-span"><i>n</i></span> cards. The description of each card consists of exactly two characters. The first character shows the color (overall this position can contain five distinct letters — R, G, B, Y, W). The second character shows the card's value (a digit from 1 to 5). Borya doesn't know exact order of the cards they lie in.</p></div><div class="output-specification"><p>Print a single integer — the minimum number of hints that the other players should make.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of Borya's cards. The next line contains the descriptions of <span class="tex-span"><i>n</i></span> cards. The description of each card consists of exactly two characters. The first character shows the color (overall this position can contain five distinct letters — R, G, B, Y, W). The second character shows the card's value (a digit from 1 to 5). Borya doesn't know exact order of the cards they lie in.</p>

## Output

<p>Print a single integer — the minimum number of hints that the other players should make.</p>





```input1
2
G3 G3

```




```input2
4
G4 R4 R3 B3

```




```input3
5
B1 Y1 W1 G1 R1

```




```output1
0

```




```output2
2

```




```output3
4

```



## Note

<p>In the first sample Borya already knows for each card that it is a green three.</p><p>In the second sample we can show all fours and all red cards.</p><p>In the third sample you need to make hints about any four colors.</p>
