## Description

<div><p>The Smart Beaver from ABBYY loves puzzles. One of his favorite puzzles is the magic square. He has recently had an idea to automate the solution of this puzzle. The Beaver decided to offer this challenge to the ABBYY Cup contestants.</p><p>The magic square is a matrix of size <span class="tex-span"><i>n</i> × <i>n</i></span>. The elements of this matrix are integers. The sum of numbers in each row of the matrix is equal to some number <span class="tex-span"><i>s</i></span>. The sum of numbers in each column of the matrix is also equal to <span class="tex-span"><i>s</i></span>. In addition, the sum of the elements on the main diagonal is equal to <span class="tex-span"><i>s</i></span> and the sum of elements on the secondary diagonal is equal to <span class="tex-span"><i>s</i></span>. Examples of magic squares are given in the following figure:</p><center> <img class="tex-graphics" src="file://nBctcgcO.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-script"> Magic squares </span> </center><p>You are given a set of <span class="tex-span"><i>n</i><sup class="upper-index">2</sup></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. It is required to place these numbers into a square matrix of size <span class="tex-span"><i>n</i> × <i>n</i></span> so that they form a magic square. Note that each number must occur in the matrix exactly the same number of times as it occurs in the original set.</p><p><span class="tex-font-style-it">It is guaranteed that a solution exists!</span></p></div><div class="input-specification"><p>The first input line contains a single integer <span class="tex-span"><i>n</i></span>. The next line contains <span class="tex-span"><i>n</i><sup class="upper-index">2</sup></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">8</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>), separated by single spaces.</p><p>The input limitations for getting 20 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>n</i> ≤ 3</span> </li></ul><p>The input limitations for getting 50 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>n</i> ≤ 4</span> </li><li> It is guaranteed that there are no more than 9 distinct numbers among <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. </li></ul><p>The input limitations for getting 100 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>n</i> ≤ 4</span> </li></ul></div><div class="output-specification"><p>The first line of the output should contain a single integer <span class="tex-span"><i>s</i></span>. In each of the following <span class="tex-span"><i>n</i></span> lines print <span class="tex-span"><i>n</i></span> integers, separated by spaces and describing the resulting magic square. In the resulting magic square the sums in the rows, columns and diagonals must be equal to <span class="tex-span"><i>s</i></span>. If there are multiple solutions, you are allowed to print any of them.</p></div>

## Input

<p>The first input line contains a single integer <span class="tex-span"><i>n</i></span>. The next line contains <span class="tex-span"><i>n</i><sup class="upper-index">2</sup></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">8</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>), separated by single spaces.</p><p>The input limitations for getting 20 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>n</i> ≤ 3</span> </li></ul><p>The input limitations for getting 50 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>n</i> ≤ 4</span> </li><li> It is guaranteed that there are no more than 9 distinct numbers among <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. </li></ul><p>The input limitations for getting 100 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>n</i> ≤ 4</span> </li></ul>

## Output

<p>The first line of the output should contain a single integer <span class="tex-span"><i>s</i></span>. In each of the following <span class="tex-span"><i>n</i></span> lines print <span class="tex-span"><i>n</i></span> integers, separated by spaces and describing the resulting magic square. In the resulting magic square the sums in the rows, columns and diagonals must be equal to <span class="tex-span"><i>s</i></span>. If there are multiple solutions, you are allowed to print any of them.</p>





```input1
3
1 2 3 4 5 6 7 8 9

```




```input2
3
1 0 -1 0 2 -1 -2 0 1

```




```input3
2
5 5 5 5

```




```output1
15
2 7 6
9 5 1
4 3 8

```




```output2
0
1 0 -1
-2 0 2
1 0 -1

```




```output3
10
5 5
5 5

```


