## Description

<div><p>Gennady owns a small hotel in the countryside where he lives a peaceful life. He loves to take long walks, watch sunsets and play cards with tourists staying in his hotel. His favorite game is called "Mau-Mau".</p><p>To play Mau-Mau, you need a pack of $52$ cards. Each card has a suit (Diamonds — <span class="tex-font-style-tt">D</span>, Clubs — <span class="tex-font-style-tt">C</span>, Spades — <span class="tex-font-style-tt">S</span>, or Hearts — <span class="tex-font-style-tt">H</span>), and a rank (<span class="tex-font-style-tt">2</span>, <span class="tex-font-style-tt">3</span>, <span class="tex-font-style-tt">4</span>, <span class="tex-font-style-tt">5</span>, <span class="tex-font-style-tt">6</span>, <span class="tex-font-style-tt">7</span>, <span class="tex-font-style-tt">8</span>, <span class="tex-font-style-tt">9</span>, <span class="tex-font-style-tt">T</span>, <span class="tex-font-style-tt">J</span>, <span class="tex-font-style-tt">Q</span>, <span class="tex-font-style-tt">K</span>, or <span class="tex-font-style-tt">A</span>).</p><p>At the start of the game, there is one card on the table and you have five cards in your hand. You can play a card from your hand if and only if it has the same rank or the same suit as the card on the table.</p><p>In order to check if you'd be a good playing partner, Gennady has prepared a task for you. Given the card on the table and five cards in your hand, check if you can play at least one card.</p></div><div class="input-specification"><p>The first line of the input contains one string which describes the card on the table. The second line contains five strings which describe the cards in your hand.</p><p>Each string is two characters long. The first character denotes the rank and belongs to the set $\{{\tt 2}, {\tt 3}, {\tt 4}, {\tt 5}, {\tt 6}, {\tt 7}, {\tt 8}, {\tt 9}, {\tt T}, {\tt J}, {\tt Q}, {\tt K}, {\tt A}\}$. The second character denotes the suit and belongs to the set $\{{\tt D}, {\tt C}, {\tt S}, {\tt H}\}$.</p><p>All the cards in the input are different.</p></div><div class="output-specification"><p>If it is possible to play a card from your hand, print one word "<span class="tex-font-style-tt">YES</span>". Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p><p>You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The first line of the input contains one string which describes the card on the table. The second line contains five strings which describe the cards in your hand.</p><p>Each string is two characters long. The first character denotes the rank and belongs to the set $\{{\tt 2}, {\tt 3}, {\tt 4}, {\tt 5}, {\tt 6}, {\tt 7}, {\tt 8}, {\tt 9}, {\tt T}, {\tt J}, {\tt Q}, {\tt K}, {\tt A}\}$. The second character denotes the suit and belongs to the set $\{{\tt D}, {\tt C}, {\tt S}, {\tt H}\}$.</p><p>All the cards in the input are different.</p>

## Output

<p>If it is possible to play a card from your hand, print one word "<span class="tex-font-style-tt">YES</span>". Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p><p>You can print each letter in any case (upper or lower).</p>





```input1
AS
2H 4C TH JH AD
```




```input2
2H
3D 4C AC KD AS
```




```input3
4D
AS AC AD AH 5H
```




```output1
YES
```




```output2
NO
```




```output3
YES
```



## Note

<p>In the first example, there is an Ace of Spades (<span class="tex-font-style-tt">AS</span>) on the table. You can play an Ace of Diamonds (<span class="tex-font-style-tt">AD</span>) because both of them are Aces.</p><p>In the second example, you cannot play any card.</p><p>In the third example, you can play an Ace of Diamonds (<span class="tex-font-style-tt">AD</span>) because it has the same suit as a Four of Diamonds (<span class="tex-font-style-tt">4D</span>), which lies on the table.</p>
