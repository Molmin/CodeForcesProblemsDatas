## Description

<div><p>A star map in Berland is a checked field <span class="tex-span"><i>n</i> × <i>m</i></span> squares. In each square there is or there is not a star. The favourite constellation of all Berland's astronomers is the constellation of the Cross. This constellation can be formed by any 5 stars so, that for some integer <span class="tex-span"><i>x</i></span> (<span class="tex-font-style-underline">radius of the constellation</span>) the following is true: </p><ul> <li> the 2nd is on the same vertical line as the 1st, but <span class="tex-span"><i>x</i></span> squares up </li><li> the 3rd is on the same vertical line as the 1st, but <span class="tex-span"><i>x</i></span> squares down </li><li> the 4th is on the same horizontal line as the 1st, but <span class="tex-span"><i>x</i></span> squares left </li><li> the 5th is on the same horizontal line as the 1st, but <span class="tex-span"><i>x</i></span> squares right </li></ul><p>Such constellations can be very numerous, that's why they are numbered with integers from 1 on the following principle: when two constellations are compared, the one with a smaller radius gets a smaller index; if their radii are equal — the one, whose central star if higher than the central star of the other one; if their central stars are at the same level — the one, whose central star is to the left of the central star of the other one.</p><p>Your task is to find the constellation with index <span class="tex-span"><i>k</i></span> by the given Berland's star map.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 300, 1 ≤ <i>k</i> ≤ 3·10<sup class="upper-index">7</sup></span>) — height and width of the map and index of the required constellation respectively. The upper-left corner has coordinates <span class="tex-span">(1, 1)</span>, and the lower-right — <span class="tex-span">(<i>n</i>, <i>m</i>)</span>. Then there follow <span class="tex-span"><i>n</i></span> lines, <span class="tex-span"><i>m</i></span> characters each — description of the map. <span class="tex-span"><i>j</i></span>-th character in <span class="tex-span"><i>i</i></span>-th line is «*», if there is a star in the corresponding square, and «.» if this square is empty.</p></div><div class="output-specification"><p>If the number of the constellations is less than <span class="tex-span"><i>k</i></span>, output <span class="tex-font-style-tt">-1</span>. Otherwise output 5 lines, two integers each — coordinates of the required constellation. Output the stars in the following order: central, upper, lower, left, right.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 300, 1 ≤ <i>k</i> ≤ 3·10<sup class="upper-index">7</sup></span>) — height and width of the map and index of the required constellation respectively. The upper-left corner has coordinates <span class="tex-span">(1, 1)</span>, and the lower-right — <span class="tex-span">(<i>n</i>, <i>m</i>)</span>. Then there follow <span class="tex-span"><i>n</i></span> lines, <span class="tex-span"><i>m</i></span> characters each — description of the map. <span class="tex-span"><i>j</i></span>-th character in <span class="tex-span"><i>i</i></span>-th line is «*», if there is a star in the corresponding square, and «.» if this square is empty.</p>

## Output

<p>If the number of the constellations is less than <span class="tex-span"><i>k</i></span>, output <span class="tex-font-style-tt">-1</span>. Otherwise output 5 lines, two integers each — coordinates of the required constellation. Output the stars in the following order: central, upper, lower, left, right.</p>





```input1
5 6 1
....*.
...***
....*.
..*...
.***..

```




```input2
5 6 2
....*.
...***
....*.
..*...
.***..

```




```input3
7 7 2
...*...
.......
...*...
*.***.*
...*...
.......
...*...

```




```output1
2 5
1 5
3 5
2 4
2 6

```




```output2
-1

```




```output3
4 4
1 4
7 4
4 1
4 7

```


