## Description

<div><p>You've got an <span class="tex-span"><i>n</i> × <i>n</i> × <i>n</i></span> cube, split into unit cubes. Your task is to number all unit cubes in this cube with positive integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i><sup class="upper-index">3</sup></span> so that: </p><ul> <li> each number was used as a cube's number exactly once; </li><li> for each <span class="tex-span">1 ≤ <i>i</i> &lt; <i>n</i><sup class="upper-index">3</sup></span>, unit cubes with numbers <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>i</i> + 1</span> were neighbouring (that is, shared a side); </li><li> for each <span class="tex-span">1 ≤ <i>i</i> &lt; <i>n</i></span> there were at least two different subcubes with sizes <span class="tex-span"><i>i</i> × <i>i</i> × <i>i</i></span>, made from unit cubes, which are numbered with consecutive numbers. That is, there are such two numbers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>, that the unit cubes of the first subcube are numbered by numbers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>x</i> + 1</span>, <span class="tex-span">...</span>, <span class="tex-span"><i>x</i> + <i>i</i><sup class="upper-index">3</sup> - 1</span>, and the unit cubes of the second subcube are numbered by numbers <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>y</i> + 1</span>, <span class="tex-span">...</span>, <span class="tex-span"><i>y</i> + <i>i</i><sup class="upper-index">3</sup> - 1</span>. </li></ul><p>Find and print the required numeration of unit cubes of the cube.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>) — the size of the cube, whose unit cubes need to be numbered.</p></div><div class="output-specification"><p>Print all layers of the cube as <span class="tex-span"><i>n</i></span> <span class="tex-span"><i>n</i> × <i>n</i></span> matrices. Separate them with new lines. Print the layers in the order in which they follow in the cube. See the samples for clarifications. </p><p>It is guaranteed that there always is a solution that meets the conditions given in the problem statement.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>) — the size of the cube, whose unit cubes need to be numbered.</p>

## Output

<p>Print all layers of the cube as <span class="tex-span"><i>n</i></span> <span class="tex-span"><i>n</i> × <i>n</i></span> matrices. Separate them with new lines. Print the layers in the order in which they follow in the cube. See the samples for clarifications. </p><p>It is guaranteed that there always is a solution that meets the conditions given in the problem statement.</p>





```input1
3

```




```output1
1 4 17 
2 3 18 
27 26 19 

8 5 16 
7 6 15 
24 25 20 

9 12 13 
10 11 14 
23 22 21 


```



## Note

<p>In the sample the cubes with sizes <span class="tex-span">2 × 2 × 2</span> are numbered with integers <span class="tex-span">1, ..., 8</span> and <span class="tex-span">5, ..., 12</span>.</p>
