## Description

<div><p>You are playing the following game. There are <span class="tex-span"><i>n</i></span> points on a plane. They are the vertices of a regular <span class="tex-span"><i>n</i></span>-polygon. Points are labeled with integer numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Each pair of distinct points is connected by a diagonal, which is colored in one of 26 colors. Points are denoted by lowercase English letters. There are three stones positioned on three distinct vertices. All stones are the same. With one move you can move the stone to another free vertex along some diagonal. The color of this diagonal must be the same as the color of the diagonal, connecting another two stones. </p><p>Your goal is to move stones in such way that the only vertices occupied by stones are <span class="tex-span">1</span>, <span class="tex-span">2</span> and <span class="tex-span">3</span>. You must achieve such position using minimal number of moves. Write a program which plays this game in an optimal way.</p></div><div class="input-specification"><p>In the first line there is one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 70</span>) — the number of points. In the second line there are three space-separated integer from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> — numbers of vertices, where stones are initially located.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>n</i></span> symbols — the matrix denoting the colors of the diagonals. Colors are denoted by lowercase English letters. The symbol <span class="tex-span"><i>j</i></span> of line <span class="tex-span"><i>i</i></span> denotes the color of diagonal between points <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span>. Matrix is symmetric, so <span class="tex-span"><i>j</i></span>-th symbol of <span class="tex-span"><i>i</i></span>-th line is equal to <span class="tex-span"><i>i</i></span>-th symbol of <span class="tex-span"><i>j</i></span>-th line. Main diagonal is filled with '<span class="tex-font-style-tt">*</span>' symbols because there is no diagonal, connecting point to itself.</p></div><div class="output-specification"><p>If there is no way to put stones on vertices <span class="tex-span">1</span>, <span class="tex-span">2</span> and <span class="tex-span">3</span>, print <span class="tex-font-style-tt">-1</span> on a single line. Otherwise, on the first line print minimal required number of moves and in the next lines print the description of each move, one move per line. To describe a move print two integers. The point from which to remove the stone, and the point to which move the stone. If there are several optimal solutions, print any of them.</p></div>

## Input

<p>In the first line there is one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 70</span>) — the number of points. In the second line there are three space-separated integer from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> — numbers of vertices, where stones are initially located.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>n</i></span> symbols — the matrix denoting the colors of the diagonals. Colors are denoted by lowercase English letters. The symbol <span class="tex-span"><i>j</i></span> of line <span class="tex-span"><i>i</i></span> denotes the color of diagonal between points <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span>. Matrix is symmetric, so <span class="tex-span"><i>j</i></span>-th symbol of <span class="tex-span"><i>i</i></span>-th line is equal to <span class="tex-span"><i>i</i></span>-th symbol of <span class="tex-span"><i>j</i></span>-th line. Main diagonal is filled with '<span class="tex-font-style-tt">*</span>' symbols because there is no diagonal, connecting point to itself.</p>

## Output

<p>If there is no way to put stones on vertices <span class="tex-span">1</span>, <span class="tex-span">2</span> and <span class="tex-span">3</span>, print <span class="tex-font-style-tt">-1</span> on a single line. Otherwise, on the first line print minimal required number of moves and in the next lines print the description of each move, one move per line. To describe a move print two integers. The point from which to remove the stone, and the point to which move the stone. If there are several optimal solutions, print any of them.</p>





```input1
4
2 3 4
*aba
a*ab
ba*b
abb*

```




```input2
4
2 3 4
*abc
a*ab
ba*b
cbb*

```




```output1
1
4 1

```




```output2
-1

```



## Note

<p>In the first example we can move stone from point <span class="tex-span">4</span> to point <span class="tex-span">1</span> because this points are connected by the diagonal of color '<span class="tex-font-style-tt">a</span>' and the diagonal connection point <span class="tex-span">2</span> and <span class="tex-span">3</span>, where the other stones are located, are connected by the diagonal of the same color. After that stones will be on the points <span class="tex-span">1</span>, <span class="tex-span">2</span> and <span class="tex-span">3</span>.</p>
