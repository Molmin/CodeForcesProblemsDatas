## Description

<div><p>The Old City is a rectangular city represented as an <span class="tex-span"><i>m</i> × <i>n</i></span> grid of blocks. This city contains many buildings, straight two-way streets and junctions. Each junction and each building is exactly one block. All the streets have width of one block and are either vertical or horizontal. There is a junction on both sides of each street. We call two blocks adjacent if and only if they share a common side. No two blocks of different streets are adjacent and no two junctions are adjacent. </p><p>There is an annual festival and as a part of it, The Old Peykan follows a special path in the city. This path starts from a block in a street, continues with many junctions and ends in a block of some street. For each street block, we know how much time it takes for the Old Peykan to go from this block to an adjacent block. Also the Old Peykan can go from each junction to its adjacent street blocks in one minute. Of course Old Peykan can't go to building blocks.</p><p>We know the initial position of the Old Peykan and the sequence of junctions that it passes to reach its destination. After passing all the junctions and reaching the destination, it will stay there forever. Your task is to find out where will the Old Peykan be <span class="tex-span"><i>k</i></span> minutes after it starts moving. Consider that The Old Peykan always follows the shortest path that passes through the given sequence of junctions and reaches the destination.</p><p>Note that the Old Peykan may visit some blocks more than once.</p></div><div class="input-specification"><p>The first line of input contains three integers <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(3 ≤ <i>m</i>, <i>n</i> ≤ 100, 1 ≤ <i>k</i> ≤ 100000)</span>. Next <span class="tex-span"><i>m</i></span> lines are representing the city's map. Each of them containts <span class="tex-span"><i>n</i></span> characters, each character is a block:</p><ul> <li> Character "<span class="tex-font-style-tt">#</span>" represents a building. </li><li> Digits "<span class="tex-font-style-tt">1</span>", "<span class="tex-font-style-tt">2</span>", <span class="tex-span">...</span>, "<span class="tex-font-style-tt">9</span>" represent a block of an street and this digit means the number of minutes it takes for the Old Peykan to pass this block. </li><li> Characters "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>", <span class="tex-span">...</span>, "<span class="tex-font-style-tt">z</span>" means that this block is a junction and this character is it's name. All the junction names are unique. </li></ul><p>Consider that all blocks have the coordinates: the <span class="tex-span"><i>j</i></span>-th in the <span class="tex-span"><i>i</i></span>-th line have coordinates <span class="tex-span">(<i>i</i>, <i>j</i>)</span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>m</i>, 1 ≤ <i>j</i> ≤ <i>n</i>)</span>.</p><p>The <span class="tex-span">(<i>m</i> + 2)</span>th line contains two integers <span class="tex-span"><i>r</i><sub class="lower-index"><i>s</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>s</i></sub></span> <span class="tex-span">(1 ≤ <i>r</i><sub class="lower-index"><i>s</i></sub> ≤ <i>m</i>, 1 ≤ <i>c</i><sub class="lower-index"><i>s</i></sub> ≤ <i>n</i>)</span>, string <span class="tex-span"><i>s</i></span> and another two integers <span class="tex-span"><i>r</i><sub class="lower-index"><i>e</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>e</i></sub></span> <span class="tex-span">(1 ≤ <i>r</i><sub class="lower-index"><i>e</i></sub> ≤ <i>m</i>, 1 ≤ <i>c</i><sub class="lower-index"><i>e</i></sub> ≤ <i>n</i>)</span>. The path starts from block <span class="tex-span">(<i>r</i><sub class="lower-index"><i>s</i></sub>, <i>c</i><sub class="lower-index"><i>s</i></sub>)</span>, continues through junctions in the order that is specified by <span class="tex-span"><i>s</i></span> and will end in block <span class="tex-span">(<i>r</i><sub class="lower-index"><i>e</i></sub>, <i>c</i><sub class="lower-index"><i>e</i></sub>)</span>. Length of <span class="tex-span"><i>s</i></span> is between <span class="tex-span">1</span> and <span class="tex-span">1000</span>.</p><p>It's guaranteed that string <span class="tex-span"><i>s</i></span> denotes a correct path from the start position to the end position and string <span class="tex-span"><i>s</i></span> doesn't contain two consecutive equal letters. Also start position <span class="tex-span">(<i>r</i><sub class="lower-index"><i>s</i></sub>, <i>c</i><sub class="lower-index"><i>s</i></sub>)</span> and the end position <span class="tex-span">(<i>r</i><sub class="lower-index"><i>e</i></sub>, <i>c</i><sub class="lower-index"><i>e</i></sub>)</span> are street blocks.</p></div><div class="output-specification"><p>In a single line print two integers <span class="tex-span"><i>r</i><sub class="lower-index"><i>f</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>f</i></sub></span> — (<span class="tex-span"><i>r</i><sub class="lower-index"><i>f</i></sub>, <i>c</i><sub class="lower-index"><i>f</i></sub></span>) being the position of the Old Peykan after exactly <span class="tex-span"><i>k</i></span> minutes.</p></div>

## Input

<p>The first line of input contains three integers <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(3 ≤ <i>m</i>, <i>n</i> ≤ 100, 1 ≤ <i>k</i> ≤ 100000)</span>. Next <span class="tex-span"><i>m</i></span> lines are representing the city's map. Each of them containts <span class="tex-span"><i>n</i></span> characters, each character is a block:</p><ul> <li> Character "<span class="tex-font-style-tt">#</span>" represents a building. </li><li> Digits "<span class="tex-font-style-tt">1</span>", "<span class="tex-font-style-tt">2</span>", <span class="tex-span">...</span>, "<span class="tex-font-style-tt">9</span>" represent a block of an street and this digit means the number of minutes it takes for the Old Peykan to pass this block. </li><li> Characters "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>", <span class="tex-span">...</span>, "<span class="tex-font-style-tt">z</span>" means that this block is a junction and this character is it's name. All the junction names are unique. </li></ul><p>Consider that all blocks have the coordinates: the <span class="tex-span"><i>j</i></span>-th in the <span class="tex-span"><i>i</i></span>-th line have coordinates <span class="tex-span">(<i>i</i>, <i>j</i>)</span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>m</i>, 1 ≤ <i>j</i> ≤ <i>n</i>)</span>.</p><p>The <span class="tex-span">(<i>m</i> + 2)</span>th line contains two integers <span class="tex-span"><i>r</i><sub class="lower-index"><i>s</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>s</i></sub></span> <span class="tex-span">(1 ≤ <i>r</i><sub class="lower-index"><i>s</i></sub> ≤ <i>m</i>, 1 ≤ <i>c</i><sub class="lower-index"><i>s</i></sub> ≤ <i>n</i>)</span>, string <span class="tex-span"><i>s</i></span> and another two integers <span class="tex-span"><i>r</i><sub class="lower-index"><i>e</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>e</i></sub></span> <span class="tex-span">(1 ≤ <i>r</i><sub class="lower-index"><i>e</i></sub> ≤ <i>m</i>, 1 ≤ <i>c</i><sub class="lower-index"><i>e</i></sub> ≤ <i>n</i>)</span>. The path starts from block <span class="tex-span">(<i>r</i><sub class="lower-index"><i>s</i></sub>, <i>c</i><sub class="lower-index"><i>s</i></sub>)</span>, continues through junctions in the order that is specified by <span class="tex-span"><i>s</i></span> and will end in block <span class="tex-span">(<i>r</i><sub class="lower-index"><i>e</i></sub>, <i>c</i><sub class="lower-index"><i>e</i></sub>)</span>. Length of <span class="tex-span"><i>s</i></span> is between <span class="tex-span">1</span> and <span class="tex-span">1000</span>.</p><p>It's guaranteed that string <span class="tex-span"><i>s</i></span> denotes a correct path from the start position to the end position and string <span class="tex-span"><i>s</i></span> doesn't contain two consecutive equal letters. Also start position <span class="tex-span">(<i>r</i><sub class="lower-index"><i>s</i></sub>, <i>c</i><sub class="lower-index"><i>s</i></sub>)</span> and the end position <span class="tex-span">(<i>r</i><sub class="lower-index"><i>e</i></sub>, <i>c</i><sub class="lower-index"><i>e</i></sub>)</span> are street blocks.</p>

## Output

<p>In a single line print two integers <span class="tex-span"><i>r</i><sub class="lower-index"><i>f</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>f</i></sub></span> — (<span class="tex-span"><i>r</i><sub class="lower-index"><i>f</i></sub>, <i>c</i><sub class="lower-index"><i>f</i></sub></span>) being the position of the Old Peykan after exactly <span class="tex-span"><i>k</i></span> minutes.</p>





```input1
3 10 12
##########
#z1a1111b#
##########
2 3 ab 2 8

```




```input2
10 3 5
###
#w#
#1#
#a#
#1#
#1#
#1#
#1#
#b#
###
3 2 abababababababab 6 2

```




```input3
3 10 6
##########
#z1a1311b#
##########
2 3 ab 2 8

```




```output1
2 8

```




```output2
8 2

```




```output3
2 7

```


