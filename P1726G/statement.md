## Description

<div><p>There are $n$ people at a party. The $i$-th person has an amount of happiness $a_i$.</p><p>Every person has a certain kind of personality which can be represented as a binary integer $b$. If $b = 0$, it means the happiness of the person will increase if he tells the story to someone <span class="tex-font-style-bf">strictly less</span> happy than them. If $b = 1$, it means the happiness of the person will increase if he tells the story to someone <span class="tex-font-style-bf">strictly more</span> happy than them.</p><p>Let us define a <span class="tex-font-style-it">speaking order</span> as an ordering of the people from left to right. Now the following process occurs. We go from left to right. The current person tells the story to all people other than himself. Note that <span class="tex-font-style-bf">all happiness values stay constant</span> while this happens. After the person is done, he counts the number of people who currently have strictly less/more happiness than him as per his kind of personality, and his happiness increases by that value. Note that only the current person's happiness value increases.</p><p>As the organizer of the party, you don't want anyone to leave sad. Therefore, you want to count the number of speaking orders such that at the end of the process <span class="tex-font-style-bf">all</span> $n$ people have <span class="tex-font-style-bf">equal</span> happiness.</p><p>Two speaking orders are considered different if there exists at least one person who does not have the same position in the two speaking orders.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \leq n \leq 2 \cdot 10^5$)&nbsp;— the number of people.</p><p>The second line contains a sequence of $n$ integers $a_1,a_2,...,a_n$ ($1 \leq a_i \leq 2n$) &nbsp;— the happiness values.</p><p>The third line contains a sequence of $n$ binary numbers $b_1,b_2,...,b_n$ ($b_i \in \{0,1\}$) &nbsp;— the kinds of personality.</p></div><div class="output-specification"><p>Output the number of different valid speaking orders. Since this number can be large, output it modulo $998244353$.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \leq n \leq 2 \cdot 10^5$)&nbsp;— the number of people.</p><p>The second line contains a sequence of $n$ integers $a_1,a_2,...,a_n$ ($1 \leq a_i \leq 2n$) &nbsp;— the happiness values.</p><p>The third line contains a sequence of $n$ binary numbers $b_1,b_2,...,b_n$ ($b_i \in \{0,1\}$) &nbsp;— the kinds of personality.</p>

## Output

<p>Output the number of different valid speaking orders. Since this number can be large, output it modulo $998244353$.</p>





```input1
4
1 2 4 4
1 1 0 0
```




```input2
4
3 4 3 1
0 1 0 0
```




```input3
21
1 2 19 19 19 19 19 19 19 19 19 21 21 21 21 21 21 21 21 21 21
1 1 0 0 0 0 0 0 0 0 0 1 1 1 1 1 1 1 1 1 1
```




```output1
2
```




```output2
0
```




```output3
49439766
```



## Note

<p>Here is the explanation for the first example. One valid speaking order is $[2,1,4,3]$ (here, we have written the indices of each person). Each step shows the current happiness values and results.</p><p>Step $1$: $[1,2,4,4]$ $\rightarrow$ Person $2$ tells the story to others. Since his kind of personality is $1$, his happiness increases by $2$ since persons $3$ and $4$ have strictly greater happiness.</p><p>Step $2$: $[1,4,4,4]$ $\rightarrow$ Person $1$ tells the story to others. Since his kind of personality is $1$, his happiness increases by $3$ since persons $2$, $3$ and $4$ have strictly greater happiness.</p><p>Step $3$: $[4,4,4,4]$ $\rightarrow$ Person $4$ tells the story to others. Since his kind of personality is $0$, his happiness increases by $0$ since no one has strictly lesser happiness.</p><p>Step $4$: $[4,4,4,4]$ $\rightarrow$ Person $3$ tells the story to others. Since his kind of personality is $0$, his happiness increases by $0$ since no one has strictly lesser happiness.</p><p>At the end, everyone has equal happiness.</p><p>Note that $[2,1,3,4]$ is also a valid answer for this example.</p><p>It can be shown that there is no valid ordering for the second example.</p>
