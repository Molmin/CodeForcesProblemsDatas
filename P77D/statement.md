## Description

<div><p><span class="tex-font-style-it">...Mike the TV greets you again!</span> </p><p><span class="tex-font-style-it">Tired of the monotonous furniture? Sick of gray routine? Dreaming about dizzying changes in your humble abode? We have something to offer you!</span> </p><p><span class="tex-font-style-it">This domino carpet for only $99.99 will change your life! You can lay it on the floor, hang it on the wall or even on the ceiling! Among other things ...</span> </p><p>Having watched the commercial, virus Hexadecimal also wanted to get a Domino Carpet and wanted badly to be photographed in front of it. But of course, a virus will never consent to buying a licensed Carpet! So she ordered a truck of dominoes and decided to make such a Carpet herself. </p><p>The original Domino Carpet is a field of squares <span class="tex-span"><i>n</i> × <i>m</i></span> in size. Each square is half of a domino, and can be rotated either vertically or horizontally, independently from its neighbors. Vertically rotated domino halves look like this: </p><center> <img class="tex-graphics" src="file://7LYAICI5.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> <p>And horizontally rotated halves look like this: </p><center> <img class="tex-graphics" src="file://1voJhJGc.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Notice, that some halves looks the same in both rotations, but other halves differ.</p><p>Dominoes bought by Hexadecimal are represented by uncuttable chips <span class="tex-span">1 × 2</span> in size, which can be laid either vertically or horizontally. If the chip is laid vertically, then both of it's halves should be laid vertically orientated; if the chip is laid horizontally, then both of it's halves should be laid horizontally.</p><p>The samples of valid and invalid dominoes laid vertically and horizontally are: </p><center> <img class="tex-graphics" src="file://fslse4Fz.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> <p>Virus Hexadecimal assembles her own Domino Carpet so that the following conditions are satisfied:</p><ul> <li> each carpet square is covered by a domino chip, i.e. there are no empty squares; </li><li> all domino chips lie entirely within the carpet and don't overlap with each other; </li><li> if there is a horizontal domino chip with its left half in column <span class="tex-span"><i>j</i></span> then there are no horizontal domino chips with their left halves in columns <span class="tex-span"><i>j</i> - 1</span> or <span class="tex-span"><i>j</i> + 1</span>. </li></ul><p>Before starting to assemble her own Domino Carpet, the virus wants to know the number of ways to achieve the intended purpose modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p><p>You can assume that the virus has an infinitely large number of dominoes of each type.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>, separated by a space — the size of the Domino Carpet (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 250</span>). Next <span class="tex-span">4<i>n</i> + 1</span> lines contain <span class="tex-span">4<i>m</i> + 1</span> symbols. </p><p>Each square of the Domino Carpet, which is a domino half, is described by a <span class="tex-span">3 × 3</span> square. Symbol <span class="tex-font-style-tt">'O'</span> in this square indicates the presence of a point, symbol <span class="tex-font-style-tt">'.'</span> — its absence. </p><p>Each <span class="tex-span">3 × 3</span> square is delineated from adjacent squares by symbols <span class="tex-font-style-tt">'#'</span> as shown in the examples. </p><p>It is guaranteed that every box describes the correct half of a domino. </p><p>In all pretests the Domino Carpets have the size of <span class="tex-span">2 × 2</span> and <span class="tex-span">4 × 4</span>.</p></div><div class="output-specification"><p>Print a single number, the number of ways to assemble the Domino Carpet modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>, using only standard dominoes of size <span class="tex-span">1 × 2</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>, separated by a space — the size of the Domino Carpet (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 250</span>). Next <span class="tex-span">4<i>n</i> + 1</span> lines contain <span class="tex-span">4<i>m</i> + 1</span> symbols. </p><p>Each square of the Domino Carpet, which is a domino half, is described by a <span class="tex-span">3 × 3</span> square. Symbol <span class="tex-font-style-tt">'O'</span> in this square indicates the presence of a point, symbol <span class="tex-font-style-tt">'.'</span> — its absence. </p><p>Each <span class="tex-span">3 × 3</span> square is delineated from adjacent squares by symbols <span class="tex-font-style-tt">'#'</span> as shown in the examples. </p><p>It is guaranteed that every box describes the correct half of a domino. </p><p>In all pretests the Domino Carpets have the size of <span class="tex-span">2 × 2</span> and <span class="tex-span">4 × 4</span>.</p>

## Output

<p>Print a single number, the number of ways to assemble the Domino Carpet modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>, using only standard dominoes of size <span class="tex-span">1 × 2</span>.</p>





```input1
3 4
#################
#O..#...#O.O#...#
#.O.#.O.#.O.#...#
#..O#...#O.O#...#
#################
#O.O#OOO#O.O#...#
#.O.#...#...#.O.#
#O.O#OOO#O.O#...#
#################
#O.O#...#O.O#...#
#...#...#...#.O.#
#O.O#...#O.O#...#
#################

```




```input2
2 2
#########
#O.O#O.O#
#.O.#...#
#O.O#O.O#
#########
#...#O.O#
#...#...#
#...#O.O#
#########

```




```input3
2 2
#########
#..O#O..#
#...#...#
#O..#..O#
#########
#O..#..O#
#...#...#
#..O#O..#
#########

```




```output1
3
```




```output2
2
```




```output3
0
```



## Note

<p><span class="tex-font-style-bf">A note to the first example:</span> all correct ways to make Domino Carpet are represented below:</p><center> <img class="tex-graphics" src="file://MpYDFZm2.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>And this way is incorrect:</p><center> <img class="tex-graphics" src="file://UKROxjqN.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
