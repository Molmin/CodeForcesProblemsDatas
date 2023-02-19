## Description

<div><center> <img class="tex-graphics" height="378px" src="file://TaIB0z8o.png" style="max-width: 100.0%;max-height: 100.0%;" width="567px"> </center><p>William really likes the cellular automaton called "Game of Life" so he decided to make his own version. For simplicity, William decided to define his cellular automaton on an array containing $n$ cells, with each cell either being alive or dead.</p><p>Evolution of the array in William's cellular automaton occurs iteratively in the following way:</p><ul> <li> If the element is dead and it has <span class="tex-font-style-bf">exactly</span> $1$ alive neighbor <span class="tex-font-style-bf">in the current state of the array</span>, then on the next iteration it will become alive. For an element at index $i$ the neighbors would be elements with indices $i - 1$ and $i + 1$. If there is no element at that index, it is considered to be a dead neighbor. </li><li> William is a humane person so all alive elements stay alive. </li></ul><p>Check the note section for examples of the evolution.</p><p>You are given some initial state of all elements and you need to help William find the state of the array after $m$ iterations of evolution.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^3$). Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($2 \le n \le 10^3, 1 \le m \le 10^9$), which are the total number of cells in the array and the number of iterations.</p><p>The second line of each test case contains a string of length $n$ made up of characters "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">1</span>" and defines the initial state of the array. "<span class="tex-font-style-tt">1</span>" means a cell is alive and "<span class="tex-font-style-tt">0</span>" means it is dead.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^4$.</p></div><div class="output-specification"><p>In each test case output a string of length $n$, made up of characters "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">1</span>" &nbsp;— the state of the array after $m$ iterations of evolution.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^3$). Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($2 \le n \le 10^3, 1 \le m \le 10^9$), which are the total number of cells in the array and the number of iterations.</p><p>The second line of each test case contains a string of length $n$ made up of characters "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">1</span>" and defines the initial state of the array. "<span class="tex-font-style-tt">1</span>" means a cell is alive and "<span class="tex-font-style-tt">0</span>" means it is dead.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^4$.</p>

## Output

<p>In each test case output a string of length $n$, made up of characters "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">1</span>" &nbsp;— the state of the array after $m$ iterations of evolution.</p>





```input1
4
11 3
01000000001
10 2
0110100101
5 2
10101
3 100
000
```




```output1
11111001111
1110111101
10101
000
```



## Note

<p>Sequence of iterations of evolution for the first test case </p><ul> <li> <span class="tex-font-style-tt">01000000001</span> &nbsp;— initial state </li><li> <span class="tex-font-style-tt">11100000011</span> &nbsp;— first iteration of evolution </li><li> <span class="tex-font-style-tt">11110000111</span> &nbsp;— second iteration of evolution </li><li> <span class="tex-font-style-tt">11111001111</span> &nbsp;— third iteration of evolution </li></ul><p>Sequence of iterations of evolution for the second test case </p><ul> <li> <span class="tex-font-style-tt">0110100101</span> &nbsp;— initial state </li><li> <span class="tex-font-style-tt">1110111101</span> &nbsp;— first iteration of evolution </li><li> <span class="tex-font-style-tt">1110111101</span> &nbsp;— second iteration of evolution </li></ul>
