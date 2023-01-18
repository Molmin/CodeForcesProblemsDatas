## Description

<div><p>You have a set of dominoes. Each domino is a rectangular tile with a line dividing its face into two square ends. Can you put all dominoes in a line one by one from left to right so that any two dominoes touched with the sides that had the same number of points? You can rotate the dominoes, changing the left and the right side (domino "1-4" turns into "4-1").</p></div><div class="input-specification"><p>The first line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1  ≤  <i>n</i>  ≤  100</span>). Next <span class="tex-span"><i>n</i></span> lines contains the dominoes. Each of these lines contains two numbers — the number of points (spots) on the left and the right half, correspondingly. The numbers of points (spots) are non-negative integers from 0 to 6.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">No solution</span>", if it is impossible to arrange the dominoes in the required manner. If the solution exists, then describe any way to arrange the dominoes. You put the dominoes from left to right. In each of <span class="tex-span"><i>n</i></span> lines print the index of the domino to put in the corresponding position and then, after a space, character "<span class="tex-font-style-tt">+</span>" (if you don't need to turn the domino) or "<span class="tex-font-style-tt">–</span>" (if you need to turn it).</p></div>

## Input

<p>The first line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1  ≤  <i>n</i>  ≤  100</span>). Next <span class="tex-span"><i>n</i></span> lines contains the dominoes. Each of these lines contains two numbers — the number of points (spots) on the left and the right half, correspondingly. The numbers of points (spots) are non-negative integers from 0 to 6.</p>

## Output

<p>Print "<span class="tex-font-style-tt">No solution</span>", if it is impossible to arrange the dominoes in the required manner. If the solution exists, then describe any way to arrange the dominoes. You put the dominoes from left to right. In each of <span class="tex-span"><i>n</i></span> lines print the index of the domino to put in the corresponding position and then, after a space, character "<span class="tex-font-style-tt">+</span>" (if you don't need to turn the domino) or "<span class="tex-font-style-tt">–</span>" (if you need to turn it).</p>





```input1
5
1 2
2 4
2 4
6 4
2 1

```




```output1
2 -
1 -
5 -
3 +
4 -

```


