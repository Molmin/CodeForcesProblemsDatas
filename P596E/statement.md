## Description

<div><p>Wilbur the pig now wants to play with strings. He has found an <span class="tex-span"><i>n</i></span> by <span class="tex-span"><i>m</i></span> table consisting only of the digits from <span class="tex-span">0</span> to <span class="tex-span">9</span> where the rows are numbered <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> and the columns are numbered <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>. Wilbur starts at some square and makes certain moves. If he is at square (<span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>) and the digit <span class="tex-span"><i>d</i></span> (<span class="tex-span">0 ≤ <i>d</i> ≤ 9</span>) is written at position (<span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>), <span class="tex-font-style-bf">then he must</span> move to the square (<span class="tex-span"><i>x</i> + <i>a</i><sub class="lower-index"><i>d</i></sub></span>, <span class="tex-span"><i>y</i> + <i>b</i><sub class="lower-index"><i>d</i></sub></span>), if that square lies within the table, and he stays in the square (<span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>) otherwise. Before Wilbur makes a move, he can choose whether or not to write the digit written in this square on the white board. All digits written on the whiteboard form some string. Every time a new digit is written, it goes to the end of the current string.</p><p>Wilbur has <span class="tex-span"><i>q</i></span> strings that he is worried about. For each string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>, Wilbur wants to know whether there exists a starting position (<span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>) so that by making finitely many moves, Wilbur can end up with the string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> written on the white board.</p></div><div class="input-specification"><p>The first line of the input consists of three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>q</i> ≤ 200</span>)&nbsp;— the dimensions of the table and the number of strings to process, respectively.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> digits from <span class="tex-span">0</span> and <span class="tex-span">9</span> giving the table itself.</p><p>Then follow <span class="tex-span">10</span> lines. The <span class="tex-span"><i>i</i></span>-th of them contains the values <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i> - 1</sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i> - 1</sub></span> (<span class="tex-span"> - 200 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 200</span>), i.e. the vector that Wilbur uses to make a move from the square with a digit <span class="tex-span"><i>i</i> - 1</span> in it.</p><p>There are <span class="tex-span"><i>q</i></span> lines that follow. The <span class="tex-span"><i>i</i></span>-th of them will contain a string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> consisting only of digits from <span class="tex-span">0</span> to <span class="tex-span">9</span>. It is guaranteed that the total length of these <span class="tex-span"><i>q</i></span> strings won't exceed <span class="tex-span">1 000 000</span>.</p></div><div class="output-specification"><p>For each of the <span class="tex-span"><i>q</i></span> strings, print "<span class="tex-font-style-tt">YES</span>" if Wilbur can choose <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> in order to finish with this string after some finite number of moves. If it's impossible, than print "<span class="tex-font-style-tt">NO</span>" for the corresponding string.</p></div>

## Input

<p>The first line of the input consists of three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>q</i> ≤ 200</span>)&nbsp;— the dimensions of the table and the number of strings to process, respectively.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> digits from <span class="tex-span">0</span> and <span class="tex-span">9</span> giving the table itself.</p><p>Then follow <span class="tex-span">10</span> lines. The <span class="tex-span"><i>i</i></span>-th of them contains the values <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i> - 1</sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i> - 1</sub></span> (<span class="tex-span"> - 200 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 200</span>), i.e. the vector that Wilbur uses to make a move from the square with a digit <span class="tex-span"><i>i</i> - 1</span> in it.</p><p>There are <span class="tex-span"><i>q</i></span> lines that follow. The <span class="tex-span"><i>i</i></span>-th of them will contain a string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> consisting only of digits from <span class="tex-span">0</span> to <span class="tex-span">9</span>. It is guaranteed that the total length of these <span class="tex-span"><i>q</i></span> strings won't exceed <span class="tex-span">1 000 000</span>.</p>

## Output

<p>For each of the <span class="tex-span"><i>q</i></span> strings, print "<span class="tex-font-style-tt">YES</span>" if Wilbur can choose <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> in order to finish with this string after some finite number of moves. If it's impossible, than print "<span class="tex-font-style-tt">NO</span>" for the corresponding string.</p>





```input1
1 1 2
0
1 1
1 1
1 1
1 1
1 1
1 1
1 1
1 1
1 1
1 1
0000000000000
2413423432432

```




```input2
4 2 5
01
23
45
67
0 1
0 -1
0 1
0 -1
0 1
0 -1
0 1
0 -1
0 1
0 -1
0000000000
010101011101
32232232322
44343222342444324
6767

```




```output1
YES
NO

```




```output2
YES
YES
YES
NO
YES

```



## Note

<p>In the first sample, there is a <span class="tex-span">1</span> by <span class="tex-span">1</span> table consisting of the only digit <span class="tex-span">0</span>. The only move that can be made is staying on the square. The first string can be written on the white board by writing <span class="tex-span">0</span> repeatedly. The second string cannot be written as there is no <span class="tex-span">2</span> on the table.</p>
