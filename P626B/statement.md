## Description

<div><p>Catherine has a deck of <span class="tex-span"><i>n</i></span> cards, each of which is either red, green, or blue. As long as there are at least two cards left, she can do one of two actions: </p><ul> <li> take any two (not necessarily adjacent) cards with different colors and exchange them for a new card of the third color; </li><li> take any two (not necessarily adjacent) cards with the same color and exchange them for a new card with that color. </li></ul><p>She repeats this process until there is only one card left. What are the possible colors for the final card?</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200</span>)&nbsp;— the total number of cards.</p><p>The next line contains a string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span> — the colors of the cards. <span class="tex-span"><i>s</i></span> contains only the characters '<span class="tex-font-style-tt">B</span>', '<span class="tex-font-style-tt">G</span>', and '<span class="tex-font-style-tt">R</span>', representing blue, green, and red, respectively.</p></div><div class="output-specification"><p>Print a single string of up to three characters&nbsp;— the possible colors of the final card (using the same symbols as the input) in alphabetical order.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200</span>)&nbsp;— the total number of cards.</p><p>The next line contains a string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span> — the colors of the cards. <span class="tex-span"><i>s</i></span> contains only the characters '<span class="tex-font-style-tt">B</span>', '<span class="tex-font-style-tt">G</span>', and '<span class="tex-font-style-tt">R</span>', representing blue, green, and red, respectively.</p>

## Output

<p>Print a single string of up to three characters&nbsp;— the possible colors of the final card (using the same symbols as the input) in alphabetical order.</p>





```input1
2
RB

```




```input2
3
GRG

```




```input3
5
BBBBB

```




```output1
G

```




```output2
BR

```




```output3
B

```



## Note

<p>In the first sample, Catherine has one red card and one blue card, which she must exchange for a green card.</p><p>In the second sample, Catherine has two green cards and one red card. She has two options: she can exchange the two green cards for a green card, then exchange the new green card and the red card for a blue card. Alternatively, she can exchange a green and a red card for a blue card, then exchange the blue card and remaining green card for a red card.</p><p>In the third sample, Catherine only has blue cards, so she can only exchange them for more blue cards.</p>
