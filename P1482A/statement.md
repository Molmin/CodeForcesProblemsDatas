## Description

<div><p>Michael is accused of violating the social distancing rules and creating a risk of spreading coronavirus. He is now sent to prison. Luckily, Michael knows exactly what the prison looks like from the inside, especially since it's very simple.</p><p>The prison can be represented as a rectangle $a\times b$ which is divided into $ab$ cells, each representing a prison cell, common sides being the walls between cells, and sides on the perimeter being the walls leading to freedom. Before sentencing, Michael can ask his friends among the prison employees to make (very well hidden) holes in some of the walls (including walls between cells and the outermost walls). Michael wants to be able to get out of the prison after this, no matter which cell he is placed in. However, he also wants to break as few walls as possible.</p><p>Your task is to find out the smallest number of walls to be broken so that there is a path to the outside from every cell after this.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1\leq t\leq 100$)&nbsp;— the number of test cases.</p><p>Each of the following $t$ lines contains two integers $a$ and $b$ ($1\leq a, b\leq 100$), representing a corresponding test case.</p></div><div class="output-specification"><p>For each test case print the single integer on a separate line&nbsp;— the answer to the problem.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1\leq t\leq 100$)&nbsp;— the number of test cases.</p><p>Each of the following $t$ lines contains two integers $a$ and $b$ ($1\leq a, b\leq 100$), representing a corresponding test case.</p>

## Output

<p>For each test case print the single integer on a separate line&nbsp;— the answer to the problem.</p>





```input1
2
2 2
1 3
```




```output1
4
3
```



## Note

<p>Some possible escape plans for the example test cases are shown below. Broken walls are shown in gray, not broken walls are shown in black. </p><p><img class="tex-graphics" src="file://HpJMnCBT.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p><img class="tex-graphics" src="file://lCe9WWfE.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
