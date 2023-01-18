## Description

<div><p>As you might already know, space has always been a problem in ICPC Jakarta. To cope with this, ICPC Jakarta is planning to build <span class="tex-font-style-bf">two</span> new buildings. These buildings should have a shape of a rectangle of the same size. Now, their problem is to find land to build the buildings.</p><p>There are $N$ lands available for sale. The $i^{th}$ land has a rectangular shape of size $L_i \times W_i$. For a good feng shui, the building's side should be parallel to the land's sides.</p><p>One way is to build the two buildings on two different lands, one on each land (not necessarily with the same orientation). A building of size $A \times B$ can be build on the $i^{th}$ land if and only if at least one of the following is satisfied: </p><ul> <li> $A \le L_i$ and $B \le W_i$, or </li><li> $A \le W_i$ and $B \le L_i$. </li></ul> Alternatively, it is also possible to build two buildings of $A \times B$ on the $i^{th}$ land with the same orientation. Formally, it is possible to build two buildings of $A \times B$ on the $i^{th}$ land if and only if at least one of the following is satisfied: <ul> <li> $A \times 2 \le L_i$ and $B \le W_i$, or </li><li> $A \times 2 \le W_i$ and $B \le L_i$, or </li><li> $A \le L_i$ and $B \times 2 \le W_i$, or </li><li> $A \le W_i$ and $B \times 2 \le L_i$. </li></ul><p>Your task in this problem is to help ICPC Jakarta to figure out the largest possible buildings they can build given $N$ available lands. Note that ICPC Jakarta has to build two buildings of $A \times B$; output the largest possible for $A \times B$.</p></div><div class="input-specification"><p>Input begins with a line containing an integer: $N$ ($1 \le N \le 100\,000$) representing the number of available lands. The next $N$ lines each contains two integers: $L_i$ $W_i$ ($1 \le L_i, W_i \le 10^9$) representing the size of the land.</p></div><div class="output-specification"><p>Output in a line a number representing the largest building that ICPC Jakarta can build with exactly one decimal point (see sample input/output for clarity).</p></div>

## Input

<p>Input begins with a line containing an integer: $N$ ($1 \le N \le 100\,000$) representing the number of available lands. The next $N$ lines each contains two integers: $L_i$ $W_i$ ($1 \le L_i, W_i \le 10^9$) representing the size of the land.</p>

## Output

<p>Output in a line a number representing the largest building that ICPC Jakarta can build with exactly one decimal point (see sample input/output for clarity).</p>





```input1
2
5 5
3 4
```




```input2
2
2 5
4 3
```




```input3
3
10 1
9 8
7 6
```




```output1
12.5
```




```output2
8.0
```




```output3
42.0
```



## Note

<p><span class="tex-font-style-it">Explanation for the sample input/output #1</span></p><p>Two buildings of $2.5 \times 5$ can be built both on the first land.</p><p><span class="tex-font-style-it">Explanation for the sample input/output #2</span></p><p>Two buildings of $2 \times 4$ can be built each on the first and second lands.</p><p><span class="tex-font-style-it">Explanation for the sample input/output #3</span></p><p>Two buildings of $7 \times 6$ can be built each on the second and third lands.</p>
