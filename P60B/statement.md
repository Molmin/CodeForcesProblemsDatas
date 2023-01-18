## Description

<div><p>The Cereal Guy's friend Serial Guy likes to watch soap operas. An episode is about to start, and he hasn't washed his plate yet. But he decided to at least put in under the tap to be filled with water. The plate can be represented by a parallelepiped <span class="tex-span"><i>k</i> × <i>n</i> × <i>m</i></span>, that is, it has <span class="tex-span"><i>k</i></span> layers (the first layer is the upper one), each of which is a rectangle <span class="tex-span"><i>n</i> × <i>m</i></span> with empty squares ('.') and obstacles ('#'). The water can only be present in the empty squares. The tap is positioned above the square <span class="tex-span">(<i>x</i>, <i>y</i>)</span> of the first layer, it is guaranteed that this square is empty. Every minute a cubical unit of water falls into the plate. Find out in how many minutes the Serial Guy should unglue himself from the soap opera and turn the water off for it not to overfill the plate. That is, you should find the moment of time when the plate is absolutely full and is going to be overfilled in the next moment.</p><p>Note: the water fills all the area within reach (see sample 4). Water flows in <span class="tex-font-style-bf">each</span> of the 6 directions, through faces of <span class="tex-span">1 × 1 × 1</span> cubes.</p></div><div class="input-specification"><p>The first line contains three numbers <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>k</i>, <i>n</i>, <i>m</i> ≤ 10</span>) which are the sizes of the plate. Then follow <span class="tex-span"><i>k</i></span> rectangles consisting of <span class="tex-span"><i>n</i></span> lines each containing <span class="tex-span"><i>m</i></span> characters '.' or '#', which represents the "layers" of the plate in the order from the top to the bottom. The rectangles are separated by empty lines (see the samples). The last line contains <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i>, 1 ≤ <i>y</i> ≤ <i>m</i></span>) which are the tap's coordinates. <span class="tex-span"><i>x</i></span> is the number of the line and <span class="tex-span"><i>y</i></span> is the number of the column. Lines of each layer are numbered from left to right by the integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, columns of each layer are numbered from top to bottom by the integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>.</p></div><div class="output-specification"><p>The answer should contain a single number, showing in how many minutes the plate will be filled.</p></div>

## Input

<p>The first line contains three numbers <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>k</i>, <i>n</i>, <i>m</i> ≤ 10</span>) which are the sizes of the plate. Then follow <span class="tex-span"><i>k</i></span> rectangles consisting of <span class="tex-span"><i>n</i></span> lines each containing <span class="tex-span"><i>m</i></span> characters '.' or '#', which represents the "layers" of the plate in the order from the top to the bottom. The rectangles are separated by empty lines (see the samples). The last line contains <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i>, 1 ≤ <i>y</i> ≤ <i>m</i></span>) which are the tap's coordinates. <span class="tex-span"><i>x</i></span> is the number of the line and <span class="tex-span"><i>y</i></span> is the number of the column. Lines of each layer are numbered from left to right by the integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, columns of each layer are numbered from top to bottom by the integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>.</p>

## Output

<p>The answer should contain a single number, showing in how many minutes the plate will be filled.</p>





```input1
1 1 1

.

1 1

```




```input2
2 1 1

.

#

1 1

```




```input3
2 2 2

.#
##

..
..

1 1

```




```input4
3 2 2

#.
##

#.
.#

..
..

1 2

```




```input5
3 3 3

.#.
###
##.

.##
###
##.

...
...
...

1 1

```




```output1
1

```




```output2
1

```




```output3
5

```




```output4
7

```




```output5
13

```


