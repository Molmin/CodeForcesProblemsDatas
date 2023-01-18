## Description

<div><p>Bob programmed a robot to navigate through a 2d maze.</p><p>The maze has some obstacles. Empty cells are denoted by the character '<span class="tex-font-style-tt">.</span>', where obstacles are denoted by '<span class="tex-font-style-tt">#</span>'.</p><p>There is a single robot in the maze. Its start position is denoted with the character '<span class="tex-font-style-tt">S</span>'. This position has no obstacle in it. There is also a single exit in the maze. Its position is denoted with the character '<span class="tex-font-style-tt">E</span>'. This position has no obstacle in it.</p><p>The robot can only move up, left, right, or down.</p><p>When Bob programmed the robot, he wrote down a string of digits consisting of the digits 0 to 3, inclusive. He intended for each digit to correspond to a distinct direction, and the robot would follow the directions in order to reach the exit. Unfortunately, he forgot to actually assign the directions to digits.</p><p>The robot will choose some random mapping of digits to distinct directions. The robot will map distinct digits to distinct directions. The robot will then follow the instructions according to the given string in order and chosen mapping. If an instruction would lead the robot to go off the edge of the maze or hit an obstacle, the robot will crash and break down. If the robot reaches the exit at any point, then the robot will stop following any further instructions.</p><p>Bob is having trouble debugging his robot, so he would like to determine the number of mappings of digits to directions that would lead the robot to the exit.</p></div><div class="input-specification"><p>The first line of input will contain two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 50</span>), denoting the dimensions of the maze.</p><p>The next <span class="tex-span"><i>n</i></span> lines will contain exactly <span class="tex-span"><i>m</i></span> characters each, denoting the maze.</p><p>Each character of the maze will be '<span class="tex-font-style-tt">.</span>', '<span class="tex-font-style-tt">#</span>', '<span class="tex-font-style-tt">S</span>', or '<span class="tex-font-style-tt">E</span>'.</p><p>There will be exactly one '<span class="tex-font-style-tt">S</span>' and exactly one '<span class="tex-font-style-tt">E</span>' in the maze.</p><p>The last line will contain a single string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 100</span>)&nbsp;— the instructions given to the robot. Each character of <span class="tex-span"><i>s</i></span> is a digit from 0 to 3.</p></div><div class="output-specification"><p>Print a single integer, the number of mappings of digits to directions that will lead the robot to the exit.</p></div>

## Input

<p>The first line of input will contain two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 50</span>), denoting the dimensions of the maze.</p><p>The next <span class="tex-span"><i>n</i></span> lines will contain exactly <span class="tex-span"><i>m</i></span> characters each, denoting the maze.</p><p>Each character of the maze will be '<span class="tex-font-style-tt">.</span>', '<span class="tex-font-style-tt">#</span>', '<span class="tex-font-style-tt">S</span>', or '<span class="tex-font-style-tt">E</span>'.</p><p>There will be exactly one '<span class="tex-font-style-tt">S</span>' and exactly one '<span class="tex-font-style-tt">E</span>' in the maze.</p><p>The last line will contain a single string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 100</span>)&nbsp;— the instructions given to the robot. Each character of <span class="tex-span"><i>s</i></span> is a digit from 0 to 3.</p>

## Output

<p>Print a single integer, the number of mappings of digits to directions that will lead the robot to the exit.</p>





```input1
5 6
.....#
S....#
.#....
.#....
...E..
333300012

```




```input2
6 6
......
......
..SE..
......
......
......
01232123212302123021

```




```input3
5 3
...
.S.
###
.E.
...
3

```




```output1
1

```




```output2
14

```




```output3
0

```



## Note

<p>For the first sample, the only valid mapping is <img align="middle" class="tex-formula" src="file://8FInpK1S.png" style="max-width: 100.0%;max-height: 100.0%;">, where <span class="tex-span"><i>D</i></span> is down, <span class="tex-span"><i>L</i></span> is left, <span class="tex-span"><i>U</i></span> is up, <span class="tex-span"><i>R</i></span> is right.</p>
