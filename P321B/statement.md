## Description

<div><p>Fox Ciel is playing a card game with her friend Jiro.</p><p>Jiro has <span class="tex-span"><i>n</i></span> cards, each one has two attributes: <span class="tex-span"><i>position</i></span> (Attack or Defense) and <span class="tex-span"><i>strength</i></span>. Fox Ciel has <span class="tex-span"><i>m</i></span> cards, each one has these two attributes too. It's known that position of all Ciel's cards is Attack.</p><p>Now is Ciel's battle phase, Ciel can do the following operation many times:</p><ol> <li> Choose one of her cards <span class="tex-span"><i>X</i></span>. This card mustn't be chosen before. </li><li> If Jiro has no alive cards at that moment, he gets the damage equal to (<span class="tex-span"><i>X</i></span>'s strength). Otherwise, Ciel needs to choose one Jiro's alive card <span class="tex-span"><i>Y</i></span>, then: <ul> <li> If <span class="tex-span"><i>Y</i></span>'s position is Attack, then (<span class="tex-span"><i>X</i></span>'s strength) <span class="tex-span"> ≥ </span> (<span class="tex-span"><i>Y</i></span>'s strength) must hold. After this attack, card <span class="tex-span"><i>Y</i></span> dies, and Jiro gets the damage equal to (<span class="tex-span"><i>X</i></span>'s strength) - (<span class="tex-span"><i>Y</i></span>'s strength). </li><li> If <span class="tex-span"><i>Y</i></span>'s position is Defense, then (<span class="tex-span"><i>X</i></span>'s strength) <span class="tex-span"> &gt; </span> (<span class="tex-span"><i>Y</i></span>'s strength) must hold. After this attack, card <span class="tex-span"><i>Y</i></span> dies, but Jiro gets no damage. </li></ul> </li></ol><p>Ciel can end her battle phase at any moment (so, she can use not all her cards). Help the Fox to calculate the maximal sum of damage Jiro can get.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>) — the number of cards Jiro and Ciel have.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains a string <span class="tex-span"><i>position</i></span> and an integer <span class="tex-span"><i>strength</i></span> <span class="tex-span">(0 ≤ <i>strength</i> ≤ 8000)</span> — the position and strength of Jiro's current card. Position is the string "<span class="tex-font-style-tt">ATK</span>" for attack, and the string "<span class="tex-font-style-tt">DEF</span>" for defense.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains an integer <span class="tex-span"><i>strength</i></span> (<span class="tex-span">0 ≤ <i>strength</i> ≤ 8000</span>) — the strength of Ciel's current card.</p></div><div class="output-specification"><p>Output an integer: the maximal damage Jiro can get.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>) — the number of cards Jiro and Ciel have.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains a string <span class="tex-span"><i>position</i></span> and an integer <span class="tex-span"><i>strength</i></span> <span class="tex-span">(0 ≤ <i>strength</i> ≤ 8000)</span> — the position and strength of Jiro's current card. Position is the string "<span class="tex-font-style-tt">ATK</span>" for attack, and the string "<span class="tex-font-style-tt">DEF</span>" for defense.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains an integer <span class="tex-span"><i>strength</i></span> (<span class="tex-span">0 ≤ <i>strength</i> ≤ 8000</span>) — the strength of Ciel's current card.</p>

## Output

<p>Output an integer: the maximal damage Jiro can get.</p>





```input1
2 3
ATK 2000
DEF 1700
2500
2500
2500

```




```input2
3 4
ATK 10
ATK 100
ATK 1000
1
11
101
1001

```




```input3
2 4
DEF 0
ATK 0
0
0
1
1

```




```output1
3000

```




```output2
992

```




```output3
1

```



## Note

<p>In the first test case, Ciel has 3 cards with same <span class="tex-span"><i>strength</i></span>. The best strategy is as follows. First she uses one of these 3 cards to attack "ATK 2000" card first, this attack destroys that card and Jiro gets <span class="tex-span">2500 - 2000 = 500</span> damage. Then she uses the second card to destroy the "DEF 1700" card. Jiro doesn't get damage that time. Now Jiro has no cards so she can use the third card to attack and Jiro gets <span class="tex-span">2500</span> damage. So the answer is <span class="tex-span">500 + 2500 = 3000</span>.</p><p>In the second test case, she should use the "1001" card to attack the "ATK 100" card, then use the "101" card to attack the "ATK 10" card. Now Ciel still has cards but she can choose to end her battle phase. The total damage equals <span class="tex-span">(1001 - 100) + (101 - 10) = 992</span>.</p><p>In the third test case note that she can destroy the "ATK 0" card by a card with strength equal to 0, but she can't destroy a "DEF 0" card with that card.</p>
