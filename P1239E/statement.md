## Description

<div><p>Kolya has a turtle and a field of size $2 \times n$. The field rows are numbered from $1$ to $2$ from top to bottom, while the columns are numbered from $1$ to $n$ from left to right.</p><p>Suppose in each cell of the field there is a lettuce leaf. The energy value of lettuce leaf in row $i$ and column $j$ is equal to $a_{i,j}$. The turtle is initially in the top left cell and wants to reach the bottom right cell. The turtle can only move right and down and among all possible ways it will choose a way, maximizing the total energy value of lettuce leaves (in case there are several such paths, it will choose any of them).</p><p>Kolya is afraid, that if turtle will eat too much lettuce, it can be bad for its health. So he wants to reorder lettuce leaves in the field, so that the energetic cost of leaves eaten by turtle will be minimized.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($2 \le n \le 25$)&nbsp;— the length of the field.</p><p>The second line contains $n$ integers $a_{1, i}$ ($0 \le a_{1, i} \le 50\,000$), the energetic cost of lettuce leaves in the first row of the field.</p><p>The third line contains $n$ integers $a_{2, i}$ ($0 \le a_{2, i} \le 50\,000$), the energetic cost of lettuce leaves in the second row of the field.</p></div><div class="output-specification"><p>Print two lines with $n$ integers in each&nbsp;— the optimal reordering of lettuce from the input data.</p><p>In case there are several optimal ways to reorder lettuce, print any of them.</p></div>

## Input

<p>The first line contains an integer $n$ ($2 \le n \le 25$)&nbsp;— the length of the field.</p><p>The second line contains $n$ integers $a_{1, i}$ ($0 \le a_{1, i} \le 50\,000$), the energetic cost of lettuce leaves in the first row of the field.</p><p>The third line contains $n$ integers $a_{2, i}$ ($0 \le a_{2, i} \le 50\,000$), the energetic cost of lettuce leaves in the second row of the field.</p>

## Output

<p>Print two lines with $n$ integers in each&nbsp;— the optimal reordering of lettuce from the input data.</p><p>In case there are several optimal ways to reorder lettuce, print any of them.</p>





```input1
2
1 4
2 3
```




```input2
3
0 0 0
0 0 0
```




```input3
3
1 0 1
0 0 0
```




```output1
1 3 
4 2
```




```output2
0 0 0 
0 0 0
```




```output3
0 0 1
0 1 0
```



## Note

<p>In the first example, after reordering, the turtle will eat lettuce with total energetic cost $1+4+2 = 7$.</p><p>In the second example, the turtle will eat lettuce with energetic cost equal $0$.</p><p>In the third example, after reordering, the turtle will eat lettuce with total energetic cost equal $1$.</p>
