## Description

<div><p>After one of celebrations there is a stack of dirty plates in Nikita's kitchen. Nikita has to wash them and put into a dryer. In dryer, the plates should be also placed in a stack also, and the plates sizes should increase down up. The sizes of all plates are distinct.</p><p>Nikita has no so much free space, specifically, he has a place for only one more stack of plates. Therefore, he can perform only such two operations: </p><ul> <li> Take any number of plates from <span class="tex-span">1</span> to <span class="tex-span"><i>a</i></span> from the top of the dirty stack, wash them and put them to the <span class="tex-font-style-it">intermediate</span> stack. </li><li> Take any number of plates from <span class="tex-span">1</span> to <span class="tex-span"><i>b</i></span> from the top of the intermediate stack and put them to the stack in the dryer. </li></ul><p>Note that after performing each of the operations, the plates are put in the same order as they were before the operation.</p><p>You are given the sizes of the plates <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i></sub></span> in the down up order in the dirty stack, and integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. All the sizes are distinct. Write a program that determines whether or not Nikita can put the plates in increasing down up order in the dryer. If he is able to do so, the program should find some sequence of operations (not necessary optimal) to achieve it.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>, <span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>). The second line contains integers <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the sizes of the plates in down up order. All the sizes are distinct.</p></div><div class="output-specification"><p>In the first line print "<span class="tex-font-style-tt">YES</span>" if there is a solution. In this case, in the second line print integer <span class="tex-span"><i>k</i></span>&nbsp;— the number of operations. Then in <span class="tex-span"><i>k</i></span> lines print the operations, one per line. Each operation is described by two integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub></span>, where <span class="tex-span"><i>t</i><sub class="lower-index"><i>j</i></sub> = 1</span>, if the operation is to wash the top <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub></span> places from the dirty stack and put them onto the intermediate stack, and <span class="tex-span"><i>t</i><sub class="lower-index"><i>j</i></sub> = 2</span>, if the operation is to move th top <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub></span> plates from the intermediate stack to the dryer. </p><p>In case there is no solution, print single line "<span class="tex-font-style-tt">NO</span>".</p><p>If there are multiple solutions, print any of them. Note that it is not necessary to minimize the number of operations.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>, <span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>). The second line contains integers <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the sizes of the plates in down up order. All the sizes are distinct.</p>

## Output

<p>In the first line print "<span class="tex-font-style-tt">YES</span>" if there is a solution. In this case, in the second line print integer <span class="tex-span"><i>k</i></span>&nbsp;— the number of operations. Then in <span class="tex-span"><i>k</i></span> lines print the operations, one per line. Each operation is described by two integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub></span>, where <span class="tex-span"><i>t</i><sub class="lower-index"><i>j</i></sub> = 1</span>, if the operation is to wash the top <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub></span> places from the dirty stack and put them onto the intermediate stack, and <span class="tex-span"><i>t</i><sub class="lower-index"><i>j</i></sub> = 2</span>, if the operation is to move th top <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub></span> plates from the intermediate stack to the dryer. </p><p>In case there is no solution, print single line "<span class="tex-font-style-tt">NO</span>".</p><p>If there are multiple solutions, print any of them. Note that it is not necessary to minimize the number of operations.</p>





```input1
6 2 3
2 3 6 4 1 5

```




```input2
7 7 7
1 2 3 4 5 6 7

```




```input3
7 1 1
1 2 3 4 5 6 7

```




```input4
4 2 2
3 2 1 4

```




```output1
YES
8
1 2
1 1
2 1
1 2
1 1
2 1
2 1
2 3

```




```output2
YES
2
1 7
2 7

```




```output3
YES
14
1 1
1 1
1 1
1 1
1 1
1 1
1 1
2 1
2 1
2 1
2 1
2 1
2 1
2 1

```




```output4
NO

```



## Note

<p>In the first example the initial order of plates was <span class="tex-span">2, 3, 6, 4, 1, 5</span>. Here is how the stacks look like after each of the operations: </p><ul> <li> [1&nbsp;2]: Dirty stack: <span class="tex-span">6, 4, 1, 5</span>. Intermediary stack: <span class="tex-span">2, 3</span>. The dryer is empty. </li><li> [1&nbsp;1]: Dirty stack: <span class="tex-span">4, 1, 5</span>. Intermediary stack: <span class="tex-span">6, 2, 3</span>. The dryer is empty. </li><li> [2&nbsp;1]: Dirty stack: <span class="tex-span">4, 1, 5</span>. Intermediary stack: <span class="tex-span">2, 3</span>. Dryer stack: <span class="tex-span">6</span>. </li><li> [1&nbsp;2]: Dirty stack: <span class="tex-span">5</span>. Intermediary stack: <span class="tex-span">4, 1, 2, 3</span>. Dryer stack: <span class="tex-span">6</span>. </li><li> [1&nbsp;1]: There are no dirty plates. Intermediary stack: <span class="tex-span">5, 4, 1, 2, 3</span>. Dryer stack: <span class="tex-span">6</span>. </li><li> [2&nbsp;1]: There are no dirty plates. Intermediary stack: <span class="tex-span">4, 1, 2, 3</span>. Dryer stack: <span class="tex-span">5, 6</span>. </li><li> [2&nbsp;1]: There are no dirty plates. Intermediary stack: <span class="tex-span">1, 2, 3</span>. Dryer stack: <span class="tex-span">4, 5, 6</span>. </li><li> [2&nbsp;3]: All the plates are in the dryer: <span class="tex-span">1, 2, 3, 4, 5, 6</span>. </li></ul> In the second example it is possible to wash all the plates in one operation, and then move them all to the dryer.<p>This is not possible in the third example, because it is not permitted to move more than one plate at the same time. It is possible to wash plates one by one so that they are placed onto the intermediary stack in the reverse order, and then move plates one by one to the dryer. The final order is correct.</p>
