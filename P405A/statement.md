## Description

<div><p>Little Chris is bored during his physics lessons (too easy), so he has built a toy box to keep himself occupied. The box is special, since it has the ability to change gravity.</p><p>There are <span class="tex-span"><i>n</i></span> columns of toy cubes in the box arranged in a line. The <span class="tex-span"><i>i</i></span>-th column contains <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> cubes. At first, the gravity in the box is pulling the cubes downwards. When Chris switches the gravity, it begins to pull all the cubes to the right side of the box. The figure shows the initial and final configurations of the cubes in the box: the cubes that have changed their position are highlighted with orange.</p><center> <img class="tex-graphics" src="file://QiKDLjQz.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Given the initial configuration of the toy cubes in the box, find the amounts of cubes in each of the <span class="tex-span"><i>n</i></span> columns after the gravity switch!</p></div><div class="input-specification"><p>The first line of input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>), the number of the columns in the box. The next line contains <span class="tex-span"><i>n</i></span> space-separated integer numbers. The <span class="tex-span"><i>i</i></span>-th number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) denotes the number of cubes in the <span class="tex-span"><i>i</i></span>-th column.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>n</i></span> integer numbers separated by spaces, where the <span class="tex-span"><i>i</i></span>-th number is the amount of cubes in the <span class="tex-span"><i>i</i></span>-th column after the gravity switch.</p></div>

## Input

<p>The first line of input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>), the number of the columns in the box. The next line contains <span class="tex-span"><i>n</i></span> space-separated integer numbers. The <span class="tex-span"><i>i</i></span>-th number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) denotes the number of cubes in the <span class="tex-span"><i>i</i></span>-th column.</p>

## Output

<p>Output <span class="tex-span"><i>n</i></span> integer numbers separated by spaces, where the <span class="tex-span"><i>i</i></span>-th number is the amount of cubes in the <span class="tex-span"><i>i</i></span>-th column after the gravity switch.</p>





```input1
4
3 2 1 2

```




```input2
3
2 3 8

```




```output1
1 2 2 3 

```




```output2
2 3 8 

```



## Note

<p>The first example case is shown on the figure. The top cube of the first column falls to the top of the last column; the top cube of the second column falls to the top of the third column; the middle cube of the first column falls to the top of the second column.</p><p>In the second example case the gravity switch does not change the heights of the columns.</p>
