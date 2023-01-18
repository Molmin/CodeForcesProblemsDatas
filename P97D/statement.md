## Description

<div><p>The Professor has lost his home robot yet again. After some thinking Professor understood that he had left the robot in the basement.</p><p>The basement in Professor's house is represented by a rectangle <span class="tex-span"><i>n</i> × <i>m</i></span>, split into <span class="tex-span">1 × 1</span> squares. Some squares are walls which are impassable; other squares are passable. You can get from any passable square to any other passable square moving through edge-adjacent passable squares. One passable square is the exit from the basement. The robot is placed exactly in one passable square. Also the robot may be placed in the exit square.</p><p>Professor is scared of going to the dark basement looking for the robot at night. However, he has a basement plan and the robot's remote control. Using the remote, Professor can send signals to the robot to shift one square left, right, up or down. When the robot receives a signal, it moves in the required direction if the robot's neighboring square in the given direction is passable. Otherwise, the robot stays idle.</p><p>Professor wrote a sequence of <span class="tex-span"><i>k</i></span> commands on a piece of paper. He thinks that the sequence can lead the robot out of the basement, wherever it's initial position might be. Professor programmed another robot to press the required buttons on the remote according to the notes on the piece of paper. Professor was just about to run the program and go to bed, when he had an epiphany.</p><p>Executing each command takes some energy and Professor doesn't want to get huge electricity bill at the end of the month. That's why he wants to find in the sequence he has written out the minimal possible prefix that would guarantee to lead the robot out to the exit after the prefix is fulfilled. And that's the problem Professor challenges you with at this late hour.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">3 ≤ <i>n</i>, <i>m</i> ≤ 150</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>). Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> characters each — that is the Professor's basement's description: "<span class="tex-font-style-tt">#</span>" stands for a wall, "<span class="tex-font-style-tt">.</span>" stands for a passable square and "<span class="tex-font-style-tt">E</span>" stands for the exit from the basement (this square also is passable). It is possible to get from each passable square to the exit, all squares located by the <span class="tex-span"><i>n</i> × <i>m</i></span> rectangle's perimeter are the walls. Exactly one square is the exit from the basement. The last line contains <span class="tex-span"><i>k</i></span> characters, the description of the sequence of commands that Professor has written out on a piece of paper. "<span class="tex-font-style-tt">L</span>", "<span class="tex-font-style-tt">R</span>", "<span class="tex-font-style-tt">U</span>", "<span class="tex-font-style-tt">D</span>" stand for commands left, right, up and down correspondingly.</p></div><div class="output-specification"><p>Print in the output file the length of the smallest possible prefix that will lead the robot to the exit square. In other words, wherever the robot had been positioned initially, it should be positioned in the exit square <span class="tex-font-style-bf">after all</span> the commands from the prefix are fulfilled (during doing commands the robot can come and leave the exit square, but only the last position of the robot is interesting for us). If Professor is mistaken and no prefix (including the whole sequence) can bring the robot to the exit, print "-1" (without the quotes). If there is the only passable square and it is the exit, print "0" (without the quotes).</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">3 ≤ <i>n</i>, <i>m</i> ≤ 150</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>). Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> characters each — that is the Professor's basement's description: "<span class="tex-font-style-tt">#</span>" stands for a wall, "<span class="tex-font-style-tt">.</span>" stands for a passable square and "<span class="tex-font-style-tt">E</span>" stands for the exit from the basement (this square also is passable). It is possible to get from each passable square to the exit, all squares located by the <span class="tex-span"><i>n</i> × <i>m</i></span> rectangle's perimeter are the walls. Exactly one square is the exit from the basement. The last line contains <span class="tex-span"><i>k</i></span> characters, the description of the sequence of commands that Professor has written out on a piece of paper. "<span class="tex-font-style-tt">L</span>", "<span class="tex-font-style-tt">R</span>", "<span class="tex-font-style-tt">U</span>", "<span class="tex-font-style-tt">D</span>" stand for commands left, right, up and down correspondingly.</p>

## Output

<p>Print in the output file the length of the smallest possible prefix that will lead the robot to the exit square. In other words, wherever the robot had been positioned initially, it should be positioned in the exit square <span class="tex-font-style-bf">after all</span> the commands from the prefix are fulfilled (during doing commands the robot can come and leave the exit square, but only the last position of the robot is interesting for us). If Professor is mistaken and no prefix (including the whole sequence) can bring the robot to the exit, print "-1" (without the quotes). If there is the only passable square and it is the exit, print "0" (without the quotes).</p>





```input1
5 5 7
#####
#...#
#...#
#E..#
#####
UULLDDR

```




```input2
5 5 7
#####
#.#.#
#...#
#E..#
#####
UULLDDR

```




```input3
5 3 2
###
#.#
#.#
#E#
###
DD

```




```output1
6

```




```output2
-1

```




```output3
2

```


