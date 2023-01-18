## Description

<div><p>Vasily the bear has got a large square white table of <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>n</i></span> columns. The table has got a black border around this table.</p><center> <img class="tex-graphics" src="file://7dV85K4B.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-script">The example of the initial table at <span class="tex-span"><i>n</i></span> = 5.</span> </center><p>Vasily the bear wants to paint his square table in exactly <span class="tex-span"><i>k</i></span> moves. Each move is sequence of actions:</p><ol> <li> The bear chooses some square inside his table. At that the square must have a black border painted around it. Also, the square shouldn't contain a black cell. The number of cells in the square shouldn't be less than <span class="tex-span">2</span>. </li><li> The bear chooses some row and some column inside the chosen square. Then he paints each cell of this row and this column inside the chosen square. After that the rectangles, formed by the square's border and the newly painted cells, must be squares of a non-zero area. </li></ol> <center> <img class="tex-graphics" src="file://qM8qa8XH.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> <center> <span class="tex-font-size-script">An example of correct painting at <span class="tex-span"><i>n</i></span> = 7 и <span class="tex-span"><i>k</i></span> = 2.</span> </center><p>The bear already knows numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span>. Help him — find the number of ways to paint the square in exactly <span class="tex-span"><i>k</i></span> moves. Two ways to paint are called distinct if the resulting tables will differ in at least one cell. As the answer can be rather large, print the remainder after dividing it by <span class="tex-span">7340033</span>.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>q</i></span> <span class="tex-span">(1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of test data.</p><p>Each of the following <span class="tex-span"><i>q</i></span> lines contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup>, 0 ≤ <i>k</i> ≤ 1000)</span> — the size of the initial table and the number of moves for the corresponding test.</p></div><div class="output-specification"><p>For each test from the input print the answer to the problem modulo <span class="tex-span">7340033</span>. Print the answers to the tests in the order in which the tests are given in the input.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>q</i></span> <span class="tex-span">(1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of test data.</p><p>Each of the following <span class="tex-span"><i>q</i></span> lines contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup>, 0 ≤ <i>k</i> ≤ 1000)</span> — the size of the initial table and the number of moves for the corresponding test.</p>

## Output

<p>For each test from the input print the answer to the problem modulo <span class="tex-span">7340033</span>. Print the answers to the tests in the order in which the tests are given in the input.</p>





```input1
8
1 0
1 1
3 0
3 1
2 0
2 1
3 2
7 2

```




```output1
1
0
1
1
1
0
0
4

```



## Note

<p>All possible painting ways for the test <span class="tex-span"><i>n</i> = 7</span> and <span class="tex-span"><i>k</i> = 2</span> are:</p><center> <img class="tex-graphics" src="file://puJKkrpi.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
