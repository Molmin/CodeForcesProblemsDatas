## Description

<div><p>In the Bus of Characters there are $n$ rows of seat, each having $2$ seats. The width of both seats in the $i$-th row is $w_i$ centimeters. All integers $w_i$ are distinct.</p><p>Initially the bus is empty. On each of $2n$ stops one passenger enters the bus. There are two types of passengers: </p><ul> <li> an introvert always chooses a row where both seats are empty. Among these rows he chooses the one with the smallest seats width and takes one of the seats in it; </li><li> an extrovert always chooses a row where exactly one seat is occupied (by an introvert). Among these rows he chooses the one with the largest seats width and takes the vacant place in it. </li></ul><p>You are given the seats width in each row and the order the passengers enter the bus. Determine which row each passenger will take.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 200\,000$) — the number of rows in the bus.</p><p>The second line contains the sequence of integers $w_1, w_2, \dots, w_n$ ($1 \le w_i \le 10^{9}$), where $w_i$ is the width of each of the seats in the $i$-th row. It is guaranteed that all $w_i$ are <span class="tex-font-style-bf">distinct</span>.</p><p>The third line contains a string of length $2n$, consisting of digits '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>' — the description of the order the passengers enter the bus. If the $j$-th character is '<span class="tex-font-style-tt">0</span>', then the passenger that enters the bus on the $j$-th stop is an introvert. If the $j$-th character is '<span class="tex-font-style-tt">1</span>', the the passenger that enters the bus on the $j$-th stop is an extrovert. It is guaranteed that the number of extroverts <span class="tex-font-style-bf">equals</span> the number of introverts (i.&nbsp;e. both numbers equal $n$), and for each extrovert there <span class="tex-font-style-bf">always</span> is a suitable row.</p></div><div class="output-specification"><p>Print $2n$ integers — the rows the passengers will take. The order of passengers should be the same as in input.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 200\,000$) — the number of rows in the bus.</p><p>The second line contains the sequence of integers $w_1, w_2, \dots, w_n$ ($1 \le w_i \le 10^{9}$), where $w_i$ is the width of each of the seats in the $i$-th row. It is guaranteed that all $w_i$ are <span class="tex-font-style-bf">distinct</span>.</p><p>The third line contains a string of length $2n$, consisting of digits '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>' — the description of the order the passengers enter the bus. If the $j$-th character is '<span class="tex-font-style-tt">0</span>', then the passenger that enters the bus on the $j$-th stop is an introvert. If the $j$-th character is '<span class="tex-font-style-tt">1</span>', the the passenger that enters the bus on the $j$-th stop is an extrovert. It is guaranteed that the number of extroverts <span class="tex-font-style-bf">equals</span> the number of introverts (i.&nbsp;e. both numbers equal $n$), and for each extrovert there <span class="tex-font-style-bf">always</span> is a suitable row.</p>

## Output

<p>Print $2n$ integers — the rows the passengers will take. The order of passengers should be the same as in input.</p>





```input1
2
3 1
0011

```




```input2
6
10 8 9 11 13 5
010010011101

```




```output1
2 1 1 2 

```




```output2
6 6 2 3 3 1 4 4 1 2 5 5 

```



## Note

<p>In the first example the first passenger (introvert) chooses the row $2$, because it has the seats with smallest width. The second passenger (introvert) chooses the row $1$, because it is the only empty row now. The third passenger (extrovert) chooses the row $1$, because it has exactly one occupied seat and the seat width is the largest among such rows. The fourth passenger (extrovert) chooses the row $2$, because it is the only row with an empty place.</p>
