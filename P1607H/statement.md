## Description

<div><p>The chef has cooked $n$ dishes yet again: the $i$-th dish consists of $a_i$ grams of fish and $b_i$ grams of meat. </p><p>Banquet organizers consider two dishes $i$ and $j$ equal if $a_i=a_j$ and $b_i=b_j$ at the same time.</p><p>The banquet organizers estimate the <span class="tex-font-style-it">variety</span> of $n$ dishes as follows. The <span class="tex-font-style-it">variety</span> of a set of dishes is equal to the number of different dishes in it. The <span class="tex-font-style-bf">less</span> <span class="tex-font-style-it">variety</span> is, the <span class="tex-font-style-bf">better</span>.</p><p>In order to reduce the <span class="tex-font-style-it">variety</span>, a taster was invited. He will eat <span class="tex-font-style-bf">exactly</span> $m_i$ grams of food from each dish. For each dish, the taster determines separately how much fish and how much meat he will eat. The only condition is that he will eat exactly $m_i$ grams of the $i$-th dish in total.</p><p>Determine how much of what type of food the taster should eat from each dish so that the value of <span class="tex-font-style-it">variety</span> is the minimum possible. If there are several correct answers, you may output any of them.</p></div><div class="input-specification"><p>The first line of input data contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>Each test case's description is preceded by a blank line. Next comes a line that contains an integer $n$ ($1 \leq n \leq 2 \cdot 10^5$)&nbsp;— the number of dishes. Then follows $n$ lines, $i$-th of which contains three integers $a_i$, $b_i$ and $m_i$ ($0 \leq a_i, b_i \le 10^6$; $0 \le m_i \le a_i+b_i$)&nbsp;— the mass of fish in $i$-th dish, the mass of meat in $i$-th dish and how many grams in total the taster should eat in $i$-th dish.</p><p>The sum of all $n$ values for all input data sets in the test does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print on the first line the minimum value of <span class="tex-font-style-it">variety</span> that can be achieved by eating exactly $m_i$ grams of food (for all $i$ from $1$ to $n$) from a dish $i$.</p><p>Then print $n$ lines that describe a way to do this: the $i$-th line should contain two integers $x_i$ and $y_i$ ($0 \leq x_i \leq a_i$; $0 \leq y_i \leq b_i$; $x_i+y_i=m_i$), where $x_i$ is how many grams of fish the taster should eat from $i$-th dish, and $y_i$ is how many grams of meat.</p><p>If there are several ways to achieve a minimum balance, print any of them.</p></div>

## Input

<p>The first line of input data contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>Each test case's description is preceded by a blank line. Next comes a line that contains an integer $n$ ($1 \leq n \leq 2 \cdot 10^5$)&nbsp;— the number of dishes. Then follows $n$ lines, $i$-th of which contains three integers $a_i$, $b_i$ and $m_i$ ($0 \leq a_i, b_i \le 10^6$; $0 \le m_i \le a_i+b_i$)&nbsp;— the mass of fish in $i$-th dish, the mass of meat in $i$-th dish and how many grams in total the taster should eat in $i$-th dish.</p><p>The sum of all $n$ values for all input data sets in the test does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print on the first line the minimum value of <span class="tex-font-style-it">variety</span> that can be achieved by eating exactly $m_i$ grams of food (for all $i$ from $1$ to $n$) from a dish $i$.</p><p>Then print $n$ lines that describe a way to do this: the $i$-th line should contain two integers $x_i$ and $y_i$ ($0 \leq x_i \leq a_i$; $0 \leq y_i \leq b_i$; $x_i+y_i=m_i$), where $x_i$ is how many grams of fish the taster should eat from $i$-th dish, and $y_i$ is how many grams of meat.</p><p>If there are several ways to achieve a minimum balance, print any of them.</p>





```input1
5

3
10 10 2
9 9 0
10 9 1

2
3 4 1
5 1 2

3
7 2 5
6 5 4
5 5 6

1
13 42 50

5
5 7 12
3 1 4
7 3 7
0 0 0
4 1 5
```




```output1
1
1 1
0 0
1 0
2
0 1
1 1
2
3 2
0 4
1 5
1
8 42
2
5 7
3 1
4 3
0 0
4 1
```


