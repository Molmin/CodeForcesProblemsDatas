## Description

<div><p>An arithmetic progression is such a <span class="tex-font-style-bf">non-empty</span> sequence of numbers where the difference between any two successive numbers is constant. This constant number is called common difference. For example, the sequence 3, 7, 11, 15 is an arithmetic progression. The definition implies that any sequences whose length equals 1 or 2 are arithmetic and all sequences whose length equals 0 are non-arithmetic.</p><p>You are given a sequence of <span class="tex-font-style-bf">different</span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. You should either split it into two arithmetic progressions or find out that the operation is impossible to perform. Splitting assigns each member of the given sequence to one of two progressions, but the relative order of numbers does not change. Splitting is an inverse operation to <span class="tex-font-style-it">merging</span>.</p></div><div class="input-specification"><p>The first line contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 30000</span>), <span class="tex-span"><i>n</i></span> is the length of the given sequence. The second line contains elements of the given sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">8</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>). The elements of the progression are different integers.</p></div><div class="output-specification"><p>Print the required arithmetic progressions, one per line. The progressions can be positioned in any order. Each progression should contain at least one number. If there's no solution, then print "No solution" (without the quotes)in the only line of the input file. If there are several solutions, print any of them.</p></div>

## Input

<p>The first line contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 30000</span>), <span class="tex-span"><i>n</i></span> is the length of the given sequence. The second line contains elements of the given sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">8</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>). The elements of the progression are different integers.</p>

## Output

<p>Print the required arithmetic progressions, one per line. The progressions can be positioned in any order. Each progression should contain at least one number. If there's no solution, then print "No solution" (without the quotes)in the only line of the input file. If there are several solutions, print any of them.</p>





```input1
6
4 1 2 7 3 10

```




```input2
5
1 2 3 -2 -7

```




```output1
1 2 3 
4 7 10 

```




```output2
1 2 3 
-2 -7 

```



## Note

<p>In the second sample another solution is also possible (number three can be assigned to the second progression): 1, 2 and 3, -2, -7.</p>
