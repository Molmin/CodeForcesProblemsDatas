## Description

<div><p>During the breaks between competitions, top-model Izabella tries to develop herself and not to be bored. For example, now she tries to solve Rubik's cube 2x2x2.</p><p>It's too hard to learn to solve Rubik's cube instantly, so she learns to understand if it's possible to solve the cube in some state using 90-degrees rotation of one face of the cube in any direction.</p><p>To check her answers she wants to use a program which will for some state of cube tell if it's possible to solve it using one rotation, described above.</p><p>Cube is called solved if for each face of cube all squares on it has the same color.</p><p><a>https://en.wikipedia.org/wiki/Rubik's_Cube</a></p></div><div class="input-specification"><p>In first line given a sequence of 24 integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 6</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> denotes color of <span class="tex-span"><i>i</i></span>-th square. There are exactly 4 occurrences of all colors in this sequence.</p></div><div class="output-specification"><p>Print «<span class="tex-font-style-tt">YES</span>» (without quotes) if it's possible to solve cube using one rotation and «<span class="tex-font-style-tt">NO</span>» (without quotes) otherwise.</p></div>

## Input

<p>In first line given a sequence of 24 integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 6</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> denotes color of <span class="tex-span"><i>i</i></span>-th square. There are exactly 4 occurrences of all colors in this sequence.</p>

## Output

<p>Print «<span class="tex-font-style-tt">YES</span>» (without quotes) if it's possible to solve cube using one rotation and «<span class="tex-font-style-tt">NO</span>» (without quotes) otherwise.</p>





```input1
2 5 4 6 1 3 6 2 5 5 1 2 3 5 3 1 1 2 4 6 6 4 3 4

```




```input2
5 3 5 3 2 5 2 5 6 2 6 2 4 4 4 4 1 1 1 1 6 3 6 3

```




```output1
NO
```




```output2
YES
```



## Note

<p>In first test case cube looks like this:</p><center> <img class="tex-graphics" src="file://51EGF13b.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In second test case cube looks like this: </p><center> <img class="tex-graphics" src="file://Zv5As16T.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>It's possible to solve cube by rotating face with squares with numbers 13, 14, 15, 16.</p>
