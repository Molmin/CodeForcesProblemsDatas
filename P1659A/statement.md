## Description

<div><p>Team Red and Team Blue competed in a competitive FPS. Their match was streamed around the world. They played a series of $n$ matches.</p><p>In the end, it turned out Team Red won $r$ times and Team Blue won $b$ times. Team Blue was less skilled than Team Red, so $b$ was <span class="tex-font-style-bf">strictly less</span> than $r$.</p><p>You missed the stream since you overslept, but you think that the match must have been neck and neck since so many people watched it. So you imagine a string of length $n$ where the $i$-th character denotes who won the $i$-th match &nbsp;— it is <span class="tex-font-style-tt">R</span> if Team Red won or <span class="tex-font-style-tt">B</span> if Team Blue won. You imagine the string was such that the <span class="tex-font-style-bf">maximum</span> number of times a team <span class="tex-font-style-bf">won in a row</span> was <span class="tex-font-style-bf">as small as possible</span>. For example, in the series of matches <span class="tex-font-style-tt">RBBRRRB</span>, Team Red won $3$ times in a row, which is the maximum.</p><p>You must find a string satisfying the above conditions. If there are multiple answers, print any.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$) &nbsp;— the number of test cases.</p><p>Each test case has a single line containing three integers $n$, $r$, and $b$ ($3 \leq n \leq 100$; $1 \leq b &lt; r \leq n$, $r+b=n$).</p></div><div class="output-specification"><p>For each test case, output a single line containing a string satisfying the given conditions. If there are multiple answers, print any.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$) &nbsp;— the number of test cases.</p><p>Each test case has a single line containing three integers $n$, $r$, and $b$ ($3 \leq n \leq 100$; $1 \leq b &lt; r \leq n$, $r+b=n$).</p>

## Output

<p>For each test case, output a single line containing a string satisfying the given conditions. If there are multiple answers, print any.</p>





```input1
3
7 4 3
6 5 1
19 13 6
```




```input2
6
3 2 1
10 6 4
11 6 5
10 9 1
10 8 2
11 9 2
```




```output1
RBRBRBR
RRRBRR
RRBRRBRRBRRBRRBRRBR
```




```output2
RBR
RRBRBRBRBR
RBRBRBRBRBR
RRRRRBRRRR
RRRBRRRBRR
RRRBRRRBRRR
```



## Note

<p>The first test case of the first example gives the optimal answer for the example in the statement. The maximum number of times a team wins in a row in <span class="tex-font-style-tt">RBRBRBR</span> is $1$. We cannot minimize it any further.</p><p>The answer for the second test case of the second example is <span class="tex-font-style-tt"><span class="tex-font-style-bf"><span class="tex-font-style-underline">RR</span></span>BRBRBRBR</span>. The maximum number of times a team wins in a row is $2$, given by <span class="tex-font-style-tt">RR</span> at the beginning. We cannot minimize the answer any further.</p>
