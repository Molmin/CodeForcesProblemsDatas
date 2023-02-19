## Description

<div><p><span class="tex-font-style-bf">It is the hard version of the problem. The only difference is that in this version $1 \le n \le 300$.</span></p><p>In the cinema seats can be represented as the table with $n$ rows and $m$ columns. The rows are numbered with integers from $1$ to $n$. The seats in each row are numbered with consecutive integers from left to right: in the $k$-th row from $m (k - 1) + 1$ to $m k$ for all rows $1 \le k \le n$.</p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$2$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\cdots$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$m - 1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$m$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$m + 1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$m + 2$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\cdots$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$2 m - 1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$2 m$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$2m + 1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$2m + 2$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\cdots$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$3 m - 1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$3 m$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\vdots$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\vdots$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\ddots$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\vdots$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\vdots$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$m (n - 1) + 1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$m (n - 1) + 2$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\cdots$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$n m - 1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$n m$</td></tr></tbody></table> <span class="tex-font-size-small">The table with seats indices</span> </center><p>There are $nm$ people who want to go to the cinema to watch a new film. They are numbered with integers from $1$ to $nm$. You should give exactly one seat to each person.</p><p>It is known, that in this cinema as lower seat index you have as better you can see everything happening on the screen. $i$-th person has the level of sight $a_i$. Let's define $s_i$ as the seat index, that will be given to $i$-th person. You want to give better places for people with lower sight levels, so for any two people $i$, $j$ such that $a_i &lt; a_j$ it should be satisfied that $s_i &lt; s_j$.</p><p>After you will give seats to all people they will start coming to their seats. In the order from $1$ to $nm$, each person will enter the hall and sit in their seat. To get to their place, the person will go to their seat's row and start moving from the first seat in this row to theirs from left to right. While moving some places will be free, some will be occupied with people already seated. The <span class="tex-font-style-bf">inconvenience</span> of the person is equal to the number of occupied seats he or she will go through.</p><p>Let's consider an example: $m = 5$, the person has the seat $4$ in the first row, the seats $1$, $3$, $5$ in the first row are already occupied, the seats $2$ and $4$ are free. The inconvenience of this person will be $2$, because he will go through occupied seats $1$ and $3$.</p><p>Find the minimal total inconvenience (the sum of inconveniences of all people), that is possible to have by giving places for all people (all conditions should be satisfied).</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n, m \le 300$)&nbsp;— the number of rows and places in each row respectively.</p><p>The second line of each test case contains $n \cdot m$ integers $a_1, a_2, \ldots, a_{n \cdot m}$ ($1 \le a_i \le 10^9$), where $a_i$ is the sight level of $i$-th person.</p><p>It's guaranteed that the sum of $n \cdot m$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case print a single integer&nbsp;— the minimal total inconvenience that can be achieved.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n, m \le 300$)&nbsp;— the number of rows and places in each row respectively.</p><p>The second line of each test case contains $n \cdot m$ integers $a_1, a_2, \ldots, a_{n \cdot m}$ ($1 \le a_i \le 10^9$), where $a_i$ is the sight level of $i$-th person.</p><p>It's guaranteed that the sum of $n \cdot m$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case print a single integer&nbsp;— the minimal total inconvenience that can be achieved.</p>





```input1
7
1 2
1 2
3 2
1 1 2 2 3 3
3 3
3 4 4 1 1 1 1 1 2
2 2
1 1 2 1
4 2
50 50 50 50 3 50 50 50
4 2
6 6 6 6 2 2 9 6
2 9
1 3 3 3 3 3 1 1 3 1 3 1 1 3 3 1 1 3
```




```output1
1
0
4
0
0
0
1
```



## Note

<p>In the first test case, there is a single way to give seats: the first person sits in the first place and the second person&nbsp;— in the second. The total inconvenience is $1$.</p><p>In the second test case the optimal seating looks like this: </p><center> <img class="tex-graphics" src="file://ac6hZrFE.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the third test case the optimal seating looks like this: </p><center> <img class="tex-graphics" src="file://6z0rsKg7.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The number in a cell is the person's index that sits on this place.</p>
