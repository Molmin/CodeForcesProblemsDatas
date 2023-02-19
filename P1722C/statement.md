## Description

<div><p>Three guys play a game: first, each person writes down $n$ distinct words of length $3$. Then, they total up the number of points as follows: </p><ul> <li> if a word was written by one person&nbsp;— that person gets 3 points, </li><li> if a word was written by two people&nbsp;— each of the two gets 1 point, </li><li> if a word was written by all&nbsp;— nobody gets any points. </li></ul> In the end, how many points does each player have?</div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 1000$)&nbsp;— the number of words written by each person.</p><p>The following three lines each contain $n$ <span class="tex-font-style-bf">distinct</span> strings&nbsp;— the words written by each person. Each string consists of $3$ lowercase English characters.</p></div><div class="output-specification"><p>For each test case, output three space-separated integers&nbsp;— the number of points each of the three guys earned. You should output the answers in the same order as the input; the $i$-th integer should be the number of points earned by the $i$-th guy.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 1000$)&nbsp;— the number of words written by each person.</p><p>The following three lines each contain $n$ <span class="tex-font-style-bf">distinct</span> strings&nbsp;— the words written by each person. Each string consists of $3$ lowercase English characters.</p>

## Output

<p>For each test case, output three space-separated integers&nbsp;— the number of points each of the three guys earned. You should output the answers in the same order as the input; the $i$-th integer should be the number of points earned by the $i$-th guy.</p>





```input1|2,3,4,5,10,11,12,13
3
1
abc
def
abc
3
orz for qaq
qaq orz for
cod for ces
5
iat roc hem ica lly
bac ter iol ogi sts
bac roc lly iol iat
```




```output1
1 3 1 
2 2 6 
9 11 5
```



## Note

<p>In the first test case: </p><ul> <li> The word $\texttt{abc}$ was written by the first and third guys&nbsp;— they each get $1$ point. </li><li> The word $\texttt{def}$ was written by the second guy only&nbsp;— he gets $3$ points. </li></ul>
