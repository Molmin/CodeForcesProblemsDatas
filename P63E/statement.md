## Description

<div><p>Karlsson has visited Lillebror again. They found a box of chocolates and a big whipped cream cake at Lillebror's place. Karlsson immediately suggested to divide the sweets fairly between Lillebror and himself. Specifically, to play together a game he has just invented with the chocolates. The winner will get the cake as a reward.</p><p>The box of chocolates has the form of a hexagon. It contains 19 cells for the chocolates, some of which contain a chocolate. The players move in turns. During one move it is allowed to eat one or several chocolates that lay in the neighboring cells on one line, parallel to one of the box's sides. The picture below shows the examples of allowed moves and of an unacceptable one. The player who cannot make a move loses.</p><center> <img class="tex-graphics" src="file://QqRpmSVH.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Karlsson makes the first move as he is Lillebror's guest and not vice versa. The players play optimally. Determine who will get the cake.</p></div><div class="input-specification"><p>The input data contains 5 lines, containing 19 words consisting of one symbol. The word "<span class="tex-font-style-tt">O</span>" means that the cell contains a chocolate and a "<span class="tex-font-style-tt">.</span>" stands for an empty cell. It is guaranteed that the box contains at least one chocolate. See the examples for better understanding.</p></div><div class="output-specification"><p>If Karlsson gets the cake, print "<span class="tex-font-style-tt">Karlsson</span>" (without the quotes), otherwise print "<span class="tex-font-style-tt">Lillebror</span>" (yet again without the quotes).</p></div>

## Input

<p>The input data contains 5 lines, containing 19 words consisting of one symbol. The word "<span class="tex-font-style-tt">O</span>" means that the cell contains a chocolate and a "<span class="tex-font-style-tt">.</span>" stands for an empty cell. It is guaranteed that the box contains at least one chocolate. See the examples for better understanding.</p>

## Output

<p>If Karlsson gets the cake, print "<span class="tex-font-style-tt">Karlsson</span>" (without the quotes), otherwise print "<span class="tex-font-style-tt">Lillebror</span>" (yet again without the quotes).</p>





```input1
. . .
 . . O .
. . O O .
 . . . .
  . . .

```




```input2
. . .
 . . . O
. . . O .
 O . O .
  . O .

```




```output1
Lillebror
```




```output2
Karlsson
```


