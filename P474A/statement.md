## Description

<div><p>Our good friend Mole is trying to code a big message. He is typing on an unusual keyboard with characters arranged in following way:</p><pre class="verbatim"><br>qwertyuiop<br>asdfghjkl;<br>zxcvbnm,./<br></pre><p>Unfortunately Mole is blind, so sometimes it is problem for him to put his hands accurately. He accidentally moved both his hands with one position to the left or to the right. That means that now he presses not a button he wants, but one neighboring button (left or right, as specified in input).</p><p>We have a sequence of characters he has typed and we want to find the original message.</p></div><div class="input-specification"><p>First line of the input contains one letter describing direction of shifting (<span class="tex-font-style-tt">'L'</span> or <span class="tex-font-style-tt">'R'</span> respectively for left or right).</p><p>Second line contains a sequence of characters written by Mole. The size of this sequence will be no more than <span class="tex-span">100</span>. Sequence contains only symbols that appear on Mole's keyboard. It doesn't contain spaces as there is no space on Mole's keyboard.</p><p>It is guaranteed that even though Mole hands are moved, he is still pressing buttons on keyboard and not hitting outside it.</p></div><div class="output-specification"><p>Print a line that contains the original message.</p></div>

## Input

<p>First line of the input contains one letter describing direction of shifting (<span class="tex-font-style-tt">'L'</span> or <span class="tex-font-style-tt">'R'</span> respectively for left or right).</p><p>Second line contains a sequence of characters written by Mole. The size of this sequence will be no more than <span class="tex-span">100</span>. Sequence contains only symbols that appear on Mole's keyboard. It doesn't contain spaces as there is no space on Mole's keyboard.</p><p>It is guaranteed that even though Mole hands are moved, he is still pressing buttons on keyboard and not hitting outside it.</p>

## Output

<p>Print a line that contains the original message.</p>





```input1
R
s;;upimrrfod;pbr

```




```output1
allyouneedislove

```


