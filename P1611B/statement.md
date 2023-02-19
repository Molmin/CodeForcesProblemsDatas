## Description

<div><p>The All-Berland Team Programming Contest will take place very soon. This year, teams of four are allowed to participate.</p><p>There are $a$ programmers and $b$ mathematicians at Berland State University. How many maximum teams can be made if:</p><ul> <li> each team must consist of exactly $4$ students, </li><li> teams of $4$ mathematicians or $4$ programmers are unlikely to perform well, so the decision was made not to compose such teams. </li></ul><p>Thus, each team must have at least one programmer <span class="tex-font-style-bf">and</span> at least one mathematician.</p><p>Print the required maximum number of teams. Each person can be a member of no more than one team.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;—the number of test cases.</p><p>This is followed by descriptions of $t$ sets, one per line. Each set is given by two integers $a$ and $b$ ($0 \le a,b \le 10^9$).</p></div><div class="output-specification"><p>Print $t$ lines. Each line must contain the answer to the corresponding set of input data&nbsp;— the required maximum number of teams.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;—the number of test cases.</p><p>This is followed by descriptions of $t$ sets, one per line. Each set is given by two integers $a$ and $b$ ($0 \le a,b \le 10^9$).</p>

## Output

<p>Print $t$ lines. Each line must contain the answer to the corresponding set of input data&nbsp;— the required maximum number of teams.</p>





```input1
6
5 5
10 1
2 3
0 0
17 2
1000000000 1000000000
```




```output1
2
1
1
0
2
500000000
```



## Note

<p>In the first test case of the example, two teams can be composed. One way to compose two teams is to compose two teams of $2$ programmers and $2$ mathematicians.</p><p>In the second test case of the example, only one team can be composed: $3$ programmers and $1$ mathematician in the team.</p>
