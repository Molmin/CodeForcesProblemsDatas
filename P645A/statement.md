## Description

<div><p>Bessie the cow and her best friend Elsie each received a sliding puzzle on Pi Day. Their puzzles consist of a <span class="tex-span">2 × 2</span> grid and three tiles labeled '<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">B</span>', and '<span class="tex-font-style-tt">C</span>'. The three tiles sit on top of the grid, leaving one grid cell empty. To make a move, Bessie or Elsie can slide a tile adjacent to the empty cell into the empty cell as shown below:</p><center> <img class="tex-graphics" src="file://uMLsSg3a.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In order to determine if they are truly Best Friends For Life (BFFLs), Bessie and Elsie would like to know if there exists a sequence of moves that takes their puzzles to the same configuration (moves can be performed in both puzzles). Two puzzles are considered to be in the same configuration if each tile is on top of the same grid cell in both puzzles. Since the tiles are labeled with letters, rotations and reflections are not allowed.</p></div><div class="input-specification"><p>The first two lines of the input consist of a <span class="tex-span">2 × 2</span> grid describing the initial configuration of Bessie's puzzle. The next two lines contain a <span class="tex-span">2 × 2</span> grid describing the initial configuration of Elsie's puzzle. The positions of the tiles are labeled '<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">B</span>', and '<span class="tex-font-style-tt">C</span>', while the empty cell is labeled '<span class="tex-font-style-tt">X</span>'. It's guaranteed that both puzzles contain exactly one tile with each letter and exactly one empty position.</p></div><div class="output-specification"><p>Output "<span class="tex-font-style-tt">YES</span>"(without quotes) if the puzzles can reach the same configuration (and Bessie and Elsie are truly BFFLs). Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p></div>

## Input

<p>The first two lines of the input consist of a <span class="tex-span">2 × 2</span> grid describing the initial configuration of Bessie's puzzle. The next two lines contain a <span class="tex-span">2 × 2</span> grid describing the initial configuration of Elsie's puzzle. The positions of the tiles are labeled '<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">B</span>', and '<span class="tex-font-style-tt">C</span>', while the empty cell is labeled '<span class="tex-font-style-tt">X</span>'. It's guaranteed that both puzzles contain exactly one tile with each letter and exactly one empty position.</p>

## Output

<p>Output "<span class="tex-font-style-tt">YES</span>"(without quotes) if the puzzles can reach the same configuration (and Bessie and Elsie are truly BFFLs). Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p>





```input1
AB
XC
XB
AC

```




```input2
AB
XC
AC
BX

```




```output1
YES

```




```output2
NO

```



## Note

<p>The solution to the first sample is described by the image. All Bessie needs to do is slide her '<span class="tex-font-style-tt">A</span>' tile down.</p><p>In the second sample, the two puzzles can never be in the same configuration. Perhaps Bessie and Elsie are not meant to be friends after all...</p>
