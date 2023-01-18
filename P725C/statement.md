## Description

<div><p>Let’s define a grid to be a set of tiles with <span class="tex-span">2</span> rows and <span class="tex-span">13</span> columns. Each tile has an English letter written in it. The letters don't have to be unique: there might be two or more tiles with the same letter written on them. Here is an example of a grid:</p><center> <pre class="verbatim">ABCDEFGHIJKLM<br>NOPQRSTUVWXYZ</pre> </center><p>We say that two tiles are adjacent if they share a side or a corner. In the example grid above, the tile with the letter '<span class="tex-font-style-tt">A</span>' is adjacent only to the tiles with letters '<span class="tex-font-style-tt">B</span>', '<span class="tex-font-style-tt">N</span>', and '<span class="tex-font-style-tt">O</span>'. A tile is not adjacent to itself.</p><p>A sequence of tiles is called a path if each tile in the sequence is adjacent to the tile which follows it (except for the last tile in the sequence, which of course has no successor). In this example, "<span class="tex-font-style-tt">ABC</span>" is a path, and so is "<span class="tex-font-style-tt">KXWIHIJK</span>". "<span class="tex-font-style-tt">MAB</span>" is not a path because '<span class="tex-font-style-tt">M</span>' is not adjacent to '<span class="tex-font-style-tt">A</span>'. A single tile can be used more than once by a path (though the tile cannot occupy two consecutive places in the path because no tile is adjacent to itself).</p><p>You’re given a string <span class="tex-span"><i>s</i></span> which consists of <span class="tex-span">27</span> upper-case English letters. Each English letter <span class="tex-font-style-bf">occurs at least once</span> in <span class="tex-span"><i>s</i></span>. Find a grid that contains a path whose tiles, viewed in the order that the path visits them, form the string <span class="tex-span"><i>s</i></span>. If there’s no solution, print "<span class="tex-font-style-tt">Impossible</span>" (without the quotes).</p></div><div class="input-specification"><p>The only line of the input contains the string <span class="tex-span"><i>s</i></span>, consisting of <span class="tex-span">27</span> upper-case English letters. Each English letter occurs at least once in <span class="tex-span"><i>s</i></span>.</p></div><div class="output-specification"><p>Output two lines, each consisting of <span class="tex-span">13</span> upper-case English characters, representing the rows of the grid. If there are multiple solutions, print any of them. If there is no solution print "<span class="tex-font-style-tt">Impossible</span>".</p></div>

## Input

<p>The only line of the input contains the string <span class="tex-span"><i>s</i></span>, consisting of <span class="tex-span">27</span> upper-case English letters. Each English letter occurs at least once in <span class="tex-span"><i>s</i></span>.</p>

## Output

<p>Output two lines, each consisting of <span class="tex-span">13</span> upper-case English characters, representing the rows of the grid. If there are multiple solutions, print any of them. If there is no solution print "<span class="tex-font-style-tt">Impossible</span>".</p>





```input1
ABCDEFGHIJKLMNOPQRSGTUVWXYZ

```




```input2
BUVTYZFQSNRIWOXXGJLKACPEMDH

```




```output1
YXWVUTGHIJKLM
ZABCDEFSRQPON

```




```output2
Impossible

```


