## Description

<div><p>Cold winter evenings in Tomsk are very boring — nobody wants be on the streets at such a time. Residents of Tomsk while away the time sitting in warm apartments, inventing a lot of different games. One of such games is 'Colored Jenga'.</p><p>This game requires wooden blocks of three colors: red, green and blue. A tower of <span class="tex-span"><i>n</i></span> levels is made from them. Each level consists of three wooden blocks. The blocks in each level can be of arbitrary colors, but they are always located close and parallel to each other. An example of such a tower is shown in the figure.</p><center> <img class="tex-graphics" src="file://y3acmBSD.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The game is played by exactly one person. Every minute a player throws a special dice which has six sides. Two sides of the dice are green, two are blue, one is red and one is black. The dice shows each side equiprobably.</p><p>If the dice shows red, green or blue, the player must take any block of this color out of the tower at this minute so that the tower doesn't fall. If this is not possible, the player waits until the end of the minute, without touching the tower. He also has to wait until the end of the minute without touching the tower if the dice shows the black side. <span class="tex-font-style-bf">It is not allowed to take blocks from the top level of the tower (whether it is completed or not)</span>.</p><p>Once a player got a block out, he must put it on the top of the tower so as to form a new level or finish the upper level consisting of previously placed blocks. The newly constructed levels should have all the same properties as the initial levels. <span class="tex-font-style-bf">If the upper level is not completed, starting the new level is prohibited</span>.</p><p>For the tower not to fall, in each of the levels except for the top, there should be at least one block. Moreover, if at some of these levels there is exactly one block left and this block is not the middle block, the tower falls.</p><p>The game ends at the moment when there is no block in the tower that you can take out so that the tower doesn't fall.</p><p>Here is a wonderful game invented by the residents of the city of Tomsk. I wonder for how many minutes can the game last if the player acts optimally well? If a player acts optimally well, then at any moment he tries to choose the block he takes out so as to minimize the expected number of the game duration.</p><p>Your task is to write a program that determines the expected number of the desired amount of minutes.</p></div><div class="input-specification"><p>The first line of the input contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 6</span>) — the number of levels in the tower.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow, describing the levels of the tower from the bottom to the top (the first line is the top of the tower). Each level is described by three characters, the first and the third of them set the border blocks of the level and the second one is the middle block. The character that describes the block has one of the following values '<span class="tex-font-style-tt">R</span>' (a red block), '<span class="tex-font-style-tt">G</span>' (a green block) and '<span class="tex-font-style-tt">B</span>' (a blue block).</p></div><div class="output-specification"><p>In the only line of the output print the sought mathematical expectation value. The answer will be considered correct if its relative or absolute error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line of the input contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 6</span>) — the number of levels in the tower.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow, describing the levels of the tower from the bottom to the top (the first line is the top of the tower). Each level is described by three characters, the first and the third of them set the border blocks of the level and the second one is the middle block. The character that describes the block has one of the following values '<span class="tex-font-style-tt">R</span>' (a red block), '<span class="tex-font-style-tt">G</span>' (a green block) and '<span class="tex-font-style-tt">B</span>' (a blue block).</p>

## Output

<p>In the only line of the output print the sought mathematical expectation value. The answer will be considered correct if its relative or absolute error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
6
RGB
GRG
BBB
GGR
BRG
BRB

```




```output1
17.119213696601992

```


