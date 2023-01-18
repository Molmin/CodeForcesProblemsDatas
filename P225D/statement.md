## Description

<div><p>Let us remind you the rules of a very popular game called "Snake" (or sometimes "Boa", "Python" or "Worm").</p><p>The game field is represented by an <span class="tex-span"><i>n</i> × <i>m</i></span> rectangular table. Some squares of the field are considered impassable (walls), all other squares of the fields are passable.</p><p>You control a snake, the snake consists of segments. Each segment takes up exactly one passable square of the field, but any passable square contains at most one segment. All segments are indexed by integers from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i></span>, where <span class="tex-span"><i>k</i></span> is the snake's length. The <span class="tex-span">1</span>-th segment is the head and the <span class="tex-span"><i>k</i></span>-th segment is the tail. For any <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> &lt; <i>k</i></span>), segments with indexes <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>i</i> + 1</span> are located in the adjacent squares of the field, that is, these squares share a common side.</p><p>One of the passable field squares contains an apple. The snake's aim is to reach the apple and eat it (that is, to position its head in the square with the apple).</p><p>The snake moves throughout the game. During one move the snake can move its head to an adjacent field square. All other segments follow the head. That is, each segment number <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 &lt; <i>i</i> ≤ <i>k</i>)</span> moves to the square that has just had segment number <span class="tex-span"><i>i</i> - 1</span>. Consider that all segments including the head move simultaneously (see the second test sample). If the snake's head moves to an unpassable square or to the square, occupied by its other segment, the snake dies. That's why we will consider such moves unvalid.</p><p>Your task is to determine the minimum number of valid moves that the snake needs to reach the apple.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 15</span>) — the number of rows and columns of the game field.</p><p>Next <span class="tex-span"><i>n</i></span> lines describe the game field. Each of these lines contains <span class="tex-span"><i>m</i></span> characters. Character "<span class="tex-font-style-tt">#</span>" represents a wall, "<span class="tex-font-style-tt">.</span>" is a passable square, "<span class="tex-font-style-tt">@</span>" is an apple. The snake's first segment is represented by character "<span class="tex-font-style-tt">1</span>", the second one segment — by character "<span class="tex-font-style-tt">2</span>" and so on.</p><p>The game field description doesn't contain any characters besides "<span class="tex-font-style-tt">#</span>', "<span class="tex-font-style-tt">.</span>", "<span class="tex-font-style-tt">@</span>" and digits (except 0). It is guaranteed that the described field is correct. It is guaranteed that the described field contains exactly one apple and exactly one snake, the snake's length is at least 3 and at most 9.</p></div><div class="output-specification"><p>Print a single integer to the output — the minimum number of moves needed to reach the apple. If the snake can't reach the apple, print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 15</span>) — the number of rows and columns of the game field.</p><p>Next <span class="tex-span"><i>n</i></span> lines describe the game field. Each of these lines contains <span class="tex-span"><i>m</i></span> characters. Character "<span class="tex-font-style-tt">#</span>" represents a wall, "<span class="tex-font-style-tt">.</span>" is a passable square, "<span class="tex-font-style-tt">@</span>" is an apple. The snake's first segment is represented by character "<span class="tex-font-style-tt">1</span>", the second one segment — by character "<span class="tex-font-style-tt">2</span>" and so on.</p><p>The game field description doesn't contain any characters besides "<span class="tex-font-style-tt">#</span>', "<span class="tex-font-style-tt">.</span>", "<span class="tex-font-style-tt">@</span>" and digits (except 0). It is guaranteed that the described field is correct. It is guaranteed that the described field contains exactly one apple and exactly one snake, the snake's length is at least 3 and at most 9.</p>

## Output

<p>Print a single integer to the output — the minimum number of moves needed to reach the apple. If the snake can't reach the apple, print <span class="tex-font-style-tt">-1</span>.</p>





```input1
4 5
##...
..1#@
432#.
...#.

```




```input2
4 4
#78#
.612
.543
..@.

```




```input3
3 2
3@
2#
1#

```




```output1
4

```




```output2
6

```




```output3
-1

```


