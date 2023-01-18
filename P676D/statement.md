## Description

<div><p>Theseus has just arrived to Crete to fight Minotaur. He found a labyrinth that has a form of a rectangular field of size <span class="tex-span"><i>n</i> × <i>m</i></span> and consists of blocks of size <span class="tex-span">1 × 1</span>.</p><p><span class="tex-font-style-bf">Each</span> block of the labyrinth has a button that rotates <span class="tex-font-style-bf">all</span> blocks <span class="tex-span">90</span> degrees clockwise. Each block rotates around its center and doesn't change its position in the labyrinth. Also, each block has some number of doors (possibly none). In one minute, Theseus can either push the button in order to rotate all the blocks <span class="tex-span">90</span> degrees clockwise or pass to the neighbouring block. Theseus can go from block <span class="tex-span"><i>A</i></span> to some neighbouring block <span class="tex-span"><i>B</i></span> only if block <span class="tex-span"><i>A</i></span> has a door that leads to block <span class="tex-span"><i>B</i></span> and block <span class="tex-span"><i>B</i></span> has a door that leads to block <span class="tex-span"><i>A</i></span>.</p><p>Theseus found an entrance to labyrinth and is now located in block <span class="tex-span">(<i>x</i><sub class="lower-index"><i>T</i></sub>, <i>y</i><sub class="lower-index"><i>T</i></sub>)</span>&nbsp;— the block in the row <span class="tex-span"><i>x</i><sub class="lower-index"><i>T</i></sub></span> and column <span class="tex-span"><i>y</i><sub class="lower-index"><i>T</i></sub></span>. Theseus know that the Minotaur is hiding in block <span class="tex-span">(<i>x</i><sub class="lower-index"><i>M</i></sub>, <i>y</i><sub class="lower-index"><i>M</i></sub>)</span> and wants to know the minimum number of minutes required to get there.</p><p>Theseus is a hero, not a programmer, so he asks you to help him.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>)&nbsp;— the number of rows and the number of columns in labyrinth, respectively.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters, describing the blocks of the labyrinth. The possible characters are:</p><ul> <li> «<span class="tex-font-style-tt">+</span>» means this block has <span class="tex-span">4</span> doors (one door to each neighbouring block); </li><li> «<span class="tex-font-style-tt">-</span>» means this block has <span class="tex-span">2</span> doors&nbsp;— to the left and to the right neighbours; </li><li> «<span class="tex-font-style-tt">|</span>» means this block has <span class="tex-span">2</span> doors&nbsp;— to the top and to the bottom neighbours; </li><li> «<span class="tex-font-style-tt">^</span>» means this block has <span class="tex-span">1</span> door&nbsp;— to the top neighbour; </li><li> «<span class="tex-font-style-tt">&gt;</span>» means this block has <span class="tex-span">1</span> door&nbsp;— to the right neighbour; </li><li> «<span class="tex-font-style-tt">&lt;</span>» means this block has <span class="tex-span">1</span> door&nbsp;— to the left neighbour; </li><li> «<span class="tex-font-style-tt">v</span>» means this block has <span class="tex-span">1</span> door&nbsp;— to the bottom neighbour;</li><li> «<span class="tex-font-style-tt">L</span>» means this block has <span class="tex-span">3</span> doors&nbsp;— to all neighbours except left one; </li><li> «<span class="tex-font-style-tt">R</span>» means this block has <span class="tex-span">3</span> doors&nbsp;— to all neighbours except right one; </li><li> «<span class="tex-font-style-tt">U</span>» means this block has <span class="tex-span">3</span> doors&nbsp;— to all neighbours except top one; </li><li> «<span class="tex-font-style-tt">D</span>» means this block has <span class="tex-span">3</span> doors&nbsp;— to all neighbours except bottom one;</li><li> «<span class="tex-font-style-tt">*</span>» means this block is a wall and has no doors. </li></ul><p>Left, right, top and bottom are defined from representing labyrinth as a table, where rows are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from top to bottom and columns are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> from left to right.</p><p>Next line contains two integers&nbsp;— coordinates of the block <span class="tex-span">(<i>x</i><sub class="lower-index"><i>T</i></sub>, <i>y</i><sub class="lower-index"><i>T</i></sub>)</span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>T</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index"><i>T</i></sub> ≤ <i>m</i></span>), where Theseus is initially located.</p><p>Last line contains two integers&nbsp;— coordinates of the block <span class="tex-span">(<i>x</i><sub class="lower-index"><i>M</i></sub>, <i>y</i><sub class="lower-index"><i>M</i></sub>)</span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>M</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index"><i>M</i></sub> ≤ <i>m</i></span>), where Minotaur hides.</p><p>It's guaranteed that both the block where Theseus starts and the block where Minotaur is hiding have at least one door. Theseus and Minotaur may be initially located at the same block.</p></div><div class="output-specification"><p>If Theseus is not able to get to Minotaur, then print <span class="tex-font-style-tt">-1</span> in the only line of the output. Otherwise, print the minimum number of minutes required to get to the block where Minotaur is hiding.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>)&nbsp;— the number of rows and the number of columns in labyrinth, respectively.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters, describing the blocks of the labyrinth. The possible characters are:</p><ul> <li> «<span class="tex-font-style-tt">+</span>» means this block has <span class="tex-span">4</span> doors (one door to each neighbouring block); </li><li> «<span class="tex-font-style-tt">-</span>» means this block has <span class="tex-span">2</span> doors&nbsp;— to the left and to the right neighbours; </li><li> «<span class="tex-font-style-tt">|</span>» means this block has <span class="tex-span">2</span> doors&nbsp;— to the top and to the bottom neighbours; </li><li> «<span class="tex-font-style-tt">^</span>» means this block has <span class="tex-span">1</span> door&nbsp;— to the top neighbour; </li><li> «<span class="tex-font-style-tt">&gt;</span>» means this block has <span class="tex-span">1</span> door&nbsp;— to the right neighbour; </li><li> «<span class="tex-font-style-tt">&lt;</span>» means this block has <span class="tex-span">1</span> door&nbsp;— to the left neighbour; </li><li> «<span class="tex-font-style-tt">v</span>» means this block has <span class="tex-span">1</span> door&nbsp;— to the bottom neighbour;</li><li> «<span class="tex-font-style-tt">L</span>» means this block has <span class="tex-span">3</span> doors&nbsp;— to all neighbours except left one; </li><li> «<span class="tex-font-style-tt">R</span>» means this block has <span class="tex-span">3</span> doors&nbsp;— to all neighbours except right one; </li><li> «<span class="tex-font-style-tt">U</span>» means this block has <span class="tex-span">3</span> doors&nbsp;— to all neighbours except top one; </li><li> «<span class="tex-font-style-tt">D</span>» means this block has <span class="tex-span">3</span> doors&nbsp;— to all neighbours except bottom one;</li><li> «<span class="tex-font-style-tt">*</span>» means this block is a wall and has no doors. </li></ul><p>Left, right, top and bottom are defined from representing labyrinth as a table, where rows are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from top to bottom and columns are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> from left to right.</p><p>Next line contains two integers&nbsp;— coordinates of the block <span class="tex-span">(<i>x</i><sub class="lower-index"><i>T</i></sub>, <i>y</i><sub class="lower-index"><i>T</i></sub>)</span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>T</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index"><i>T</i></sub> ≤ <i>m</i></span>), where Theseus is initially located.</p><p>Last line contains two integers&nbsp;— coordinates of the block <span class="tex-span">(<i>x</i><sub class="lower-index"><i>M</i></sub>, <i>y</i><sub class="lower-index"><i>M</i></sub>)</span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>M</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index"><i>M</i></sub> ≤ <i>m</i></span>), where Minotaur hides.</p><p>It's guaranteed that both the block where Theseus starts and the block where Minotaur is hiding have at least one door. Theseus and Minotaur may be initially located at the same block.</p>

## Output

<p>If Theseus is not able to get to Minotaur, then print <span class="tex-font-style-tt">-1</span> in the only line of the output. Otherwise, print the minimum number of minutes required to get to the block where Minotaur is hiding.</p>





```input1
2 2
+*
*U
1 1
2 2

```




```input2
2 3
&lt;&gt;&lt;
&gt;&lt;&gt;
1 1
2 1

```




```output1
-1
```




```output2
4
```



## Note

<p>Assume that Theseus starts at the block <span class="tex-span">(<i>x</i><sub class="lower-index"><i>T</i></sub>, <i>y</i><sub class="lower-index"><i>T</i></sub>)</span> at the moment <span class="tex-span">0</span>.</p>
