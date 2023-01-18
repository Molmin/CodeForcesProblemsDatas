## Description

<div><p>Toastman came up with a very complicated task. He gives it to Appleman, but Appleman doesn't know how to solve it. Can you help him?</p><p>Given a <span class="tex-span"><i>n</i> × <i>n</i></span> checkerboard. Each cell of the board has either character '<span class="tex-font-style-tt">x</span>', or character '<span class="tex-font-style-tt">o</span>', or nothing. How many ways to fill all the empty cells with '<span class="tex-font-style-tt">x</span>' or '<span class="tex-font-style-tt">o</span>' (each cell must contain only one character in the end) are there, such that for each cell the number of adjacent cells with '<span class="tex-font-style-tt">o</span>' will be even? Find the number of ways modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>. Two cells of the board are adjacent if they share a side.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>) — the size of the board, and the number of cells that has characters initially. </p><p>Then <span class="tex-span"><i>k</i></span> lines follows. The <span class="tex-span"><i>i</i></span>-th line contains two integers and a character: <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>; <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is either '<span class="tex-font-style-tt">o</span>' or '<span class="tex-font-style-tt">x</span>'). This line means: there is a character <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> in the cell that is located on the intersection of the <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>-th row and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>-th column. All the given cells are distinct.</p><p>Consider that the rows are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from top to bottom. Analogically, the columns are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from left to right.</p></div><div class="output-specification"><p>Print a single integer — the answer to the problem.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>) — the size of the board, and the number of cells that has characters initially. </p><p>Then <span class="tex-span"><i>k</i></span> lines follows. The <span class="tex-span"><i>i</i></span>-th line contains two integers and a character: <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>; <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is either '<span class="tex-font-style-tt">o</span>' or '<span class="tex-font-style-tt">x</span>'). This line means: there is a character <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> in the cell that is located on the intersection of the <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>-th row and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>-th column. All the given cells are distinct.</p><p>Consider that the rows are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from top to bottom. Analogically, the columns are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from left to right.</p>

## Output

<p>Print a single integer — the answer to the problem.</p>





```input1
3 2
1 1 x
2 2 o

```




```input2
4 3
2 4 x
3 4 x
3 2 x

```




```output1
2

```




```output2
2

```



## Note

<p>In the first example there are two ways:</p><pre class="verbatim"><br>    xxo          xoo<br>    xox          ooo<br>    oxx          oox<br></pre>
