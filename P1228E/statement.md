## Description

<div><p>You have $n \times n$ square grid and an integer $k$. Put an integer in each cell while satisfying the conditions below.</p><ul> <li> All numbers in the grid should be between $1$ and $k$ inclusive. </li><li> Minimum number of the $i$-th row is $1$ ($1 \le i \le n$). </li><li> Minimum number of the $j$-th column is $1$ ($1 \le j \le n$). </li></ul><p>Find the number of ways to put integers in the grid. Since the answer can be very large, find the answer modulo $(10^{9} + 7)$.</p><center> <img class="tex-graphics" src="file://FiMJxN4C.png" style="max-width: 100.0%;max-height: 100.0%;"> These are the examples of valid and invalid grid when $n=k=2$. </center></div><div class="input-specification"><p>The only line contains two integers $n$ and $k$ ($1 \le n \le 250$, $1 \le k \le 10^{9}$).</p></div><div class="output-specification"><p>Print the answer modulo $(10^{9} + 7)$.</p></div>

## Input

<p>The only line contains two integers $n$ and $k$ ($1 \le n \le 250$, $1 \le k \le 10^{9}$).</p>

## Output

<p>Print the answer modulo $(10^{9} + 7)$.</p>





```input1
2 2
```




```input2
123 456789
```




```output1
7
```




```output2
689974806
```



## Note

<p>In the first example, following $7$ cases are possible.</p><center> <img class="tex-graphics" src="file://rgWrsVmT.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second example, make sure you print the answer modulo $(10^{9} + 7)$.</p>
