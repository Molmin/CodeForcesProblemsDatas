## Description

<div><p>There is a matrix <span class="tex-span"><i>A</i></span> of size <span class="tex-span"><i>x</i> × <i>y</i></span> filled with integers. For every <img align="middle" class="tex-formula" src="file://YAwqupGB.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://ejaugHBQ.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = <i>y</i>(<i>i</i> - 1) + <i>j</i></span>. Obviously, every integer from <span class="tex-span">[1..<i>xy</i>]</span> occurs exactly once in this matrix. </p><p>You have traversed some path in this matrix. Your path can be described as a sequence of visited cells <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> denoting that you started in the cell containing the number <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, then moved to the cell with the number <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, and so on.</p><p>From the cell located in <span class="tex-span"><i>i</i></span>-th line and <span class="tex-span"><i>j</i></span>-th column (we denote this cell as <span class="tex-span">(<i>i</i>, <i>j</i>)</span>) you can move into one of the following cells:</p><ol><li> <span class="tex-span">(<i>i</i> + 1, <i>j</i>)</span> — only if <span class="tex-span"><i>i</i> &lt; <i>x</i></span>; </li><li> <span class="tex-span">(<i>i</i>, <i>j</i> + 1)</span> — only if <span class="tex-span"><i>j</i> &lt; <i>y</i></span>; </li><li> <span class="tex-span">(<i>i</i> - 1, <i>j</i>)</span> — only if <span class="tex-span"><i>i</i> &gt; 1</span>; </li><li> <span class="tex-span">(<i>i</i>, <i>j</i> - 1)</span> — only if <span class="tex-span"><i>j</i> &gt; 1</span>.</li></ol><p>Notice that making a move requires you to go to an adjacent cell. It is not allowed to stay in the same cell. You don't know <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> exactly, but you have to find any possible values for these numbers such that you could start in the cell containing the integer <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, then move to the cell containing <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> (in one step), then move to the cell containing <span class="tex-span"><i>a</i><sub class="lower-index">3</sub></span> (also in one step) and so on. Can you choose <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> so that they don't contradict with your sequence of moves?</p></div><div class="input-specification"><p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200000</span>) — the number of cells you visited on your path (if some cell is visited twice, then it's listed twice).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the integers in the cells on your path.</p></div><div class="output-specification"><p>If all possible values of <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> such that <span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">9</sup></span> contradict with the information about your path, print <span class="tex-font-style-tt">NO</span>.</p><p>Otherwise, print <span class="tex-font-style-tt">YES</span> in the first line, and in the second line print the values <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> such that your path was possible with such number of lines and columns in the matrix. Remember that they must be positive integers not exceeding <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p></div>

## Input

<p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200000</span>) — the number of cells you visited on your path (if some cell is visited twice, then it's listed twice).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the integers in the cells on your path.</p>

## Output

<p>If all possible values of <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> such that <span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">9</sup></span> contradict with the information about your path, print <span class="tex-font-style-tt">NO</span>.</p><p>Otherwise, print <span class="tex-font-style-tt">YES</span> in the first line, and in the second line print the values <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> such that your path was possible with such number of lines and columns in the matrix. Remember that they must be positive integers not exceeding <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p>





```input1
8
1 2 3 6 9 8 5 2

```




```input2
6
1 2 1 2 5 3

```




```input3
2
1 10

```




```output1
YES
3 3

```




```output2
NO

```




```output3
YES
4 9

```



## Note

<p>The matrix and the path on it in the first test looks like this:</p><center> <img class="tex-graphics" src="file://nZokjeVY.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Also there exist multiple correct answers for both the first and the third examples.</p>
