## Description

<div><p>Polycarp and Monocarp are both solving the same puzzle with dominoes. They are given the same set of $n$ dominoes, the $i$-th of which contains two numbers $x_i$ and $y_i$. They are also both given the same $m$ by $k$ grid of values $a_{ij}$ such that $m\cdot k = 2n$.</p><p>The puzzle asks them to place the $n$ dominoes on the grid in such a way that none of them overlap, and the values on each domino match the $a_{ij}$ values that domino covers. Dominoes can be rotated arbitrarily before being placed on the grid, so the domino $(x_i, y_i)$ is equivalent to the domino $(y_i, x_i)$.</p><p>They have both solved the puzzle, and compared their answers, but noticed that not only did their solutions not match, but none of the $n$ dominoes were in the same location in both solutions! Formally, if two squares were covered by the same domino in Polycarp's solution, they were covered by different dominoes in Monocarp's solution. The diagram below shows one potential $a$ grid, along with the two players' solutions.</p><center> <img class="tex-graphics" src="file://b5Tv59HW.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Polycarp and Monocarp remember the set of dominoes they started with, but they have lost the grid $a$. Help them reconstruct one possible grid $a$, along with both of their solutions, or determine that no such grid exists.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 3\cdot 10^5$).</p><p>The $i$-th of the next $n$ lines contains two integers $x_i$ and $y_i$ ($1 \le x_i, y_i \le 2n$).</p></div><div class="output-specification"><p>If there is no solution, print a single integer $-1$.</p><p>Otherwise, print $m$ and $k$, the height and width of the puzzle grid, on the first line of output. These should satisfy $m\cdot k = 2n$.</p><p>The $i$-th of the next $m$ lines should contain $k$ integers, the $j$-th of which is $a_{ij}$.</p><p>The next $m$ lines describe Polycarp's solution. Print $m$ lines of $k$ characters each. For each square, if it is covered by the upper half of a domino in Polycarp's solution, it should contain a "U". Similarly, if it is covered by the bottom, left, or right half of a domino, it should contain "D", "L", or "R", respectively.</p><p>The next $m$ lines should describe Monocarp's solution, in the same format as Polycarp's solution.</p><p>If there are multiple answers, print any.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 3\cdot 10^5$).</p><p>The $i$-th of the next $n$ lines contains two integers $x_i$ and $y_i$ ($1 \le x_i, y_i \le 2n$).</p>

## Output

<p>If there is no solution, print a single integer $-1$.</p><p>Otherwise, print $m$ and $k$, the height and width of the puzzle grid, on the first line of output. These should satisfy $m\cdot k = 2n$.</p><p>The $i$-th of the next $m$ lines should contain $k$ integers, the $j$-th of which is $a_{ij}$.</p><p>The next $m$ lines describe Polycarp's solution. Print $m$ lines of $k$ characters each. For each square, if it is covered by the upper half of a domino in Polycarp's solution, it should contain a "U". Similarly, if it is covered by the bottom, left, or right half of a domino, it should contain "D", "L", or "R", respectively.</p><p>The next $m$ lines should describe Monocarp's solution, in the same format as Polycarp's solution.</p><p>If there are multiple answers, print any.</p>





```input1
1
1 2
```




```input2
2
1 1
1 2
```




```input3
10
1 3
1 1
2 1
3 4
1 5
1 5
3 1
2 4
3 3
4 1
```




```output1
-1
```




```output2
2 2

2 1
1 1

LR
LR

UU
DD
```




```output3
4 5

1 2 5 1 5
3 4 1 3 1
1 2 4 4 1
1 3 3 3 1

LRULR
LRDLR
ULRLR
DLRLR

UULRU
DDUUD
LRDDU
LRLRD
```



## Note

<p>Extra blank lines are added to the output for clarity, but are not required.</p><p>The third sample case corresponds to the image from the statement.</p>
