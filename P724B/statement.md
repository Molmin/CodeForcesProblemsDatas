## Description

<div><p>You are given a table consisting of <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns.</p><p>Numbers in each row form a permutation of integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>.</p><p>You are allowed to pick two elements in one row and swap them, but <span class="tex-font-style-bf">no more than once</span> for each row. Also, <span class="tex-font-style-bf">no more than once</span> you are allowed to pick two columns and swap them. Thus, you are allowed to perform from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i> + 1</span> actions in total. <span class="tex-font-style-bf">Operations can be performed in any order</span>.</p><p>You have to check whether it's possible to obtain the identity permutation <span class="tex-span">1, 2, ..., <i>m</i></span> in each row. In other words, check if one can perform some of the operation following the given rules and make each row sorted in increasing order.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 20</span>)&nbsp;— the number of rows and the number of columns in the given table. </p><p>Each of next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> integers&nbsp;— elements of the table. It's guaranteed that numbers in each line form a permutation of integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>.</p></div><div class="output-specification"><p>If there is a way to obtain the identity permutation in each row by following the given rules, print "<span class="tex-font-style-tt">YES</span>" (without quotes) in the only line of the output. Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 20</span>)&nbsp;— the number of rows and the number of columns in the given table. </p><p>Each of next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> integers&nbsp;— elements of the table. It's guaranteed that numbers in each line form a permutation of integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>.</p>

## Output

<p>If there is a way to obtain the identity permutation in each row by following the given rules, print "<span class="tex-font-style-tt">YES</span>" (without quotes) in the only line of the output. Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p>





```input1
2 4
1 3 2 4
1 3 4 2

```




```input2
4 4
1 2 3 4
2 3 4 1
3 4 1 2
4 1 2 3

```




```input3
3 6
2 1 3 4 5 6
1 2 4 3 5 6
1 2 3 4 6 5

```




```output1
YES

```




```output2
NO

```




```output3
YES

```



## Note

<p>In the first sample, one can act in the following way: </p><ol> <li> Swap second and third columns. Now the table is <center class="tex-equation"><span class="tex-span">1&nbsp;2&nbsp;3&nbsp;4</span></center> <center class="tex-equation"><span class="tex-span">1&nbsp;4&nbsp;3&nbsp;2</span></center> </li><li> In the second row, swap the second and the fourth elements. Now the table is <center class="tex-equation"><span class="tex-span">1&nbsp;2&nbsp;3&nbsp;4</span></center> <center class="tex-equation"><span class="tex-span">1&nbsp;2&nbsp;3&nbsp;4</span></center> </li></ol>
