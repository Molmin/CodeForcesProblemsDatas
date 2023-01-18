## Description

<div><p>ZS the Coder and Chris the Baboon arrived at the entrance of Udayland. There is a <span class="tex-span"><i>n</i> × <i>n</i></span> magic grid on the entrance which is filled with integers. Chris noticed that exactly one of the cells in the grid is empty, and to enter Udayland, they need to fill a <span class="tex-font-style-bf">positive integer</span> into the empty cell.</p><p>Chris tried filling in random numbers but it didn't work. ZS the Coder realizes that they need to fill in a positive integer such that the numbers in the grid form <span class="tex-font-style-it">a magic square</span>. This means that he has to fill in a positive integer so that the sum of the numbers in each row of the grid (<img align="middle" class="tex-formula" src="file://czidYgDF.png" style="max-width: 100.0%;max-height: 100.0%;">), each column of the grid (<img align="middle" class="tex-formula" src="file://QGWZ7is6.png" style="max-width: 100.0%;max-height: 100.0%;">), and the two long diagonals of the grid (the main diagonal&nbsp;— <img align="middle" class="tex-formula" src="file://wmC17qyq.png" style="max-width: 100.0%;max-height: 100.0%;"> and the secondary diagonal&nbsp;— <img align="middle" class="tex-formula" src="file://6w4AJKht.png" style="max-width: 100.0%;max-height: 100.0%;">) are equal. </p><p>Chris doesn't know what number to fill in. Can you help Chris find the correct positive integer to fill in or determine that it is impossible?</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500</span>)&nbsp;— the number of rows and columns of the magic grid.</p><p><span class="tex-span"><i>n</i></span> lines follow, each of them contains <span class="tex-span"><i>n</i></span> integers. The <span class="tex-span"><i>j</i></span>-th number in the <span class="tex-span"><i>i</i></span>-th of them denotes <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span> or <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = 0</span>), the number in the <span class="tex-span"><i>i</i></span>-th row and <span class="tex-span"><i>j</i></span>-th column of the magic grid. If the corresponding cell is empty, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> will be equal to <span class="tex-span">0</span>. Otherwise, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> is <span class="tex-font-style-bf">positive</span>.</p><p>It is guaranteed that there is exactly one pair of integers <span class="tex-span"><i>i</i>, <i>j</i></span> <span class="tex-span">(1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i>)</span> such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = 0</span>.</p></div><div class="output-specification"><p>Output a single integer, the positive integer <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ 10<sup class="upper-index">18</sup></span>) that should be filled in the empty cell so that the whole grid becomes a magic square. If such positive integer <span class="tex-span"><i>x</i></span> does not exist, output <span class="tex-span"> - 1</span> instead.</p><p>If there are multiple solutions, you may print any of them.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500</span>)&nbsp;— the number of rows and columns of the magic grid.</p><p><span class="tex-span"><i>n</i></span> lines follow, each of them contains <span class="tex-span"><i>n</i></span> integers. The <span class="tex-span"><i>j</i></span>-th number in the <span class="tex-span"><i>i</i></span>-th of them denotes <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span> or <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = 0</span>), the number in the <span class="tex-span"><i>i</i></span>-th row and <span class="tex-span"><i>j</i></span>-th column of the magic grid. If the corresponding cell is empty, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> will be equal to <span class="tex-span">0</span>. Otherwise, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> is <span class="tex-font-style-bf">positive</span>.</p><p>It is guaranteed that there is exactly one pair of integers <span class="tex-span"><i>i</i>, <i>j</i></span> <span class="tex-span">(1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i>)</span> such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = 0</span>.</p>

## Output

<p>Output a single integer, the positive integer <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ 10<sup class="upper-index">18</sup></span>) that should be filled in the empty cell so that the whole grid becomes a magic square. If such positive integer <span class="tex-span"><i>x</i></span> does not exist, output <span class="tex-span"> - 1</span> instead.</p><p>If there are multiple solutions, you may print any of them.</p>





```input1
3
4 0 2
3 5 7
8 1 6

```




```input2
4
1 1 1 1
1 1 0 1
1 1 1 1
1 1 1 1

```




```input3
4
1 1 1 1
1 1 0 1
1 1 2 1
1 1 1 1

```




```output1
9

```




```output2
1

```




```output3
-1

```



## Note

<p>In the first sample case, we can fill in <span class="tex-span">9</span> into the empty cell to make the resulting grid a magic square. Indeed, </p><p>The sum of numbers in each row is:</p><p><span class="tex-span">4 + 9 + 2 = 3 + 5 + 7 = 8 + 1 + 6 = 15</span>.</p><p>The sum of numbers in each column is:</p><p><span class="tex-span">4 + 3 + 8 = 9 + 5 + 1 = 2 + 7 + 6 = 15</span>.</p><p>The sum of numbers in the two diagonals is:</p><p><span class="tex-span">4 + 5 + 6 = 2 + 5 + 8 = 15</span>.</p><p>In the third sample case, it is impossible to fill a number in the empty square such that the resulting grid is a magic square.</p>
