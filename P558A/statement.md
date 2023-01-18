## Description

<div><p>Amr lives in Lala Land. Lala Land is a very beautiful country that is located on a coordinate line. Lala Land is famous with its apple trees growing everywhere.</p><p>Lala Land has exactly <span class="tex-span"><i>n</i></span> apple trees. Tree number <span class="tex-span"><i>i</i></span> is located in a position <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and has <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> apples growing on it. Amr wants to collect apples from the apple trees. Amr currently stands in <span class="tex-span"><i>x</i> = 0</span> position. At the beginning, he can choose whether to go right or left. He'll continue in his direction until he meets an apple tree he didn't visit before. He'll take all of its apples and then reverse his direction, continue walking in this direction until he meets another apple tree he didn't visit before and so on. In the other words, Amr reverses his direction when visiting each new apple tree. Amr will stop collecting apples when there are no more trees he didn't visit in the direction he is facing.</p><p>What is the maximum number of apples he can collect?</p></div><div class="input-specification"><p>The first line contains one number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>), the number of apple trees in Lala Land.</p><p>The following <span class="tex-span"><i>n</i></span> lines contains two integers each <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">5</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≠ 0</span>, <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>), representing the position of the <span class="tex-span"><i>i</i></span>-th tree and number of apples on it.</p><p>It's guaranteed that there is at most one apple tree at each coordinate. It's guaranteed that no tree grows in point <span class="tex-span">0</span>.</p></div><div class="output-specification"><p>Output the maximum number of apples Amr can collect.</p></div>

## Input

<p>The first line contains one number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>), the number of apple trees in Lala Land.</p><p>The following <span class="tex-span"><i>n</i></span> lines contains two integers each <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">5</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≠ 0</span>, <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>), representing the position of the <span class="tex-span"><i>i</i></span>-th tree and number of apples on it.</p><p>It's guaranteed that there is at most one apple tree at each coordinate. It's guaranteed that no tree grows in point <span class="tex-span">0</span>.</p>

## Output

<p>Output the maximum number of apples Amr can collect.</p>





```input1
2
-1 5
1 5

```




```input2
3
-2 2
1 4
-1 3

```




```input3
3
1 9
3 5
7 10

```




```output1
10
```




```output2
9
```




```output3
9
```



## Note

<p>In the first sample test it doesn't matter if Amr chose at first to go left or right. In both cases he'll get all the apples.</p><p>In the second sample test the optimal solution is to go left to <span class="tex-span"><i>x</i> =  - 1</span>, collect apples from there, then the direction will be reversed, Amr has to go to <span class="tex-span"><i>x</i> = 1</span>, collect apples from there, then the direction will be reversed and Amr goes to the final tree <span class="tex-span"><i>x</i> =  - 2</span>.</p><p>In the third sample test the optimal solution is to go right to <span class="tex-span"><i>x</i> = 1</span>, collect apples from there, then the direction will be reversed and Amr will not be able to collect anymore apples because there are no apple trees to his left.</p>
