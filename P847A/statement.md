## Description

<div><p>Doubly linked list is one of the fundamental data structures. A doubly linked list is a sequence of elements, each containing information about the previous and the next elements of the list. In this problem all lists have linear structure. I.e. each element except the first has exactly one previous element, each element except the last has exactly one next element. The list is not closed in a cycle.</p><p>In this problem you are given <span class="tex-span"><i>n</i></span> memory cells forming one or more doubly linked lists. Each cell contains information about element from some list. Memory cells are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p><p>For each cell <span class="tex-span"><i>i</i></span> you are given two values: </p><ul> <li> <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> — cell containing previous element for the element in the cell <span class="tex-span"><i>i</i></span>; </li><li> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> — cell containing next element for the element in the cell <span class="tex-span"><i>i</i></span>. </li></ul><p>If cell <span class="tex-span"><i>i</i></span> contains information about the element which has no previous element then <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> = 0</span>. Similarly, if cell <span class="tex-span"><i>i</i></span> contains information about the element which has no next element then <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub> = 0</span>.</p><center> <img class="tex-graphics" src="file://7rukHKOb.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">Three lists are shown on the picture.</span> </center><p>For example, for the picture above the values of <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> are the following: <span class="tex-span"><i>l</i><sub class="lower-index">1</sub> = 4</span>, <span class="tex-span"><i>r</i><sub class="lower-index">1</sub> = 7</span>; <span class="tex-span"><i>l</i><sub class="lower-index">2</sub> = 5</span>, <span class="tex-span"><i>r</i><sub class="lower-index">2</sub> = 0</span>; <span class="tex-span"><i>l</i><sub class="lower-index">3</sub> = 0</span>, <span class="tex-span"><i>r</i><sub class="lower-index">3</sub> = 0</span>; <span class="tex-span"><i>l</i><sub class="lower-index">4</sub> = 6</span>, <span class="tex-span"><i>r</i><sub class="lower-index">4</sub> = 1</span>; <span class="tex-span"><i>l</i><sub class="lower-index">5</sub> = 0</span>, <span class="tex-span"><i>r</i><sub class="lower-index">5</sub> = 2</span>; <span class="tex-span"><i>l</i><sub class="lower-index">6</sub> = 0</span>, <span class="tex-span"><i>r</i><sub class="lower-index">6</sub> = 4</span>; <span class="tex-span"><i>l</i><sub class="lower-index">7</sub> = 1</span>, <span class="tex-span"><i>r</i><sub class="lower-index">7</sub> = 0</span>.</p><p>Your task is to unite all given lists in a single list, joining them to each other in any order. In particular, if the input data already contains a single list, then there is no need to perform any actions. Print the resulting list in the form of values <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Any other action, other than joining the beginning of one list to the end of another, can not be performed.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of memory cells where the doubly linked lists are located.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the cells of the previous and the next element of list for cell <span class="tex-span"><i>i</i></span>. Value <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> = 0</span> if element in cell <span class="tex-span"><i>i</i></span> has no previous element in its list. Value <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub> = 0</span> if element in cell <span class="tex-span"><i>i</i></span> has no next element in its list.</p><p>It is guaranteed that the input contains the correct description of a single or more doubly linked lists. All lists have linear structure: each element of list except the first has exactly one previous element; each element of list except the last has exactly one next element. Each memory cell contains information about one element from some list, each element of each list written in one of <span class="tex-span"><i>n</i></span> given cells.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> lines, the <span class="tex-span"><i>i</i></span>-th line must contain two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> — the cells of the previous and the next element of list for cell <span class="tex-span"><i>i</i></span> after all lists from the input are united in a single list. If there are many solutions print any of them.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of memory cells where the doubly linked lists are located.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the cells of the previous and the next element of list for cell <span class="tex-span"><i>i</i></span>. Value <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> = 0</span> if element in cell <span class="tex-span"><i>i</i></span> has no previous element in its list. Value <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub> = 0</span> if element in cell <span class="tex-span"><i>i</i></span> has no next element in its list.</p><p>It is guaranteed that the input contains the correct description of a single or more doubly linked lists. All lists have linear structure: each element of list except the first has exactly one previous element; each element of list except the last has exactly one next element. Each memory cell contains information about one element from some list, each element of each list written in one of <span class="tex-span"><i>n</i></span> given cells.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> lines, the <span class="tex-span"><i>i</i></span>-th line must contain two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> — the cells of the previous and the next element of list for cell <span class="tex-span"><i>i</i></span> after all lists from the input are united in a single list. If there are many solutions print any of them.</p>





```input1
7
4 7
5 0
0 0
6 1
0 2
0 4
1 0

```




```output1
4 7
5 6
0 5
6 1
3 2
2 4
1 0

```


