## Description

<div><p>Dima is a beginner programmer. During his working process, he regularly has to repeat the following operation again and again: to remove every second element from the array. One day he has been bored with easy solutions of this problem, and he has come up with the following extravagant algorithm.</p><p>Let's consider that initially array contains <span class="tex-span"><i>n</i></span> numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> and the number <span class="tex-span"><i>i</i></span> is located in the cell with the index <span class="tex-span">2<i>i</i> - 1</span> (Indices are numbered starting from one) and other cells of the array are empty. Each step Dima selects a non-empty array cell with the maximum index and moves the number written in it to the nearest empty cell to the left of the selected one. The process continues until all <span class="tex-span"><i>n</i></span> numbers will appear in the first <span class="tex-span"><i>n</i></span> cells of the array. For example if <span class="tex-span"><i>n</i> = 4</span>, the array is changing as follows:</p><center> <img class="tex-graphics" src="file://mJMWiJxg.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>You have to write a program that allows you to determine what number will be in the cell with index <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span>) after Dima's algorithm finishes.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 200 000</span>), the number of elements in the array and the number of queries for which it is needed to find the answer.</p><p>Next <span class="tex-span"><i>q</i></span> lines contain integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), the indices of cells for which it is necessary to output their content after Dima's algorithm finishes.</p></div><div class="output-specification"><p>For each of <span class="tex-span"><i>q</i></span> queries output one integer number, the value that will appear in the corresponding array cell after Dima's algorithm finishes.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 200 000</span>), the number of elements in the array and the number of queries for which it is needed to find the answer.</p><p>Next <span class="tex-span"><i>q</i></span> lines contain integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), the indices of cells for which it is necessary to output their content after Dima's algorithm finishes.</p>

## Output

<p>For each of <span class="tex-span"><i>q</i></span> queries output one integer number, the value that will appear in the corresponding array cell after Dima's algorithm finishes.</p>





```input1
4 3
2
3
4

```




```input2
13 4
10
5
4
8

```




```output1
3
2
4

```




```output2
13
3
8
9

```



## Note

<p>The first example is shown in the picture.</p><p>In the second example the final array is <span class="tex-span">[1, 12, 2, 8, 3, 11, 4, 9, 5, 13, 6, 10, 7]</span>.</p>
