## Description

<div><p>Kuroni isn't good at economics. So he decided to found a new financial pyramid called <span class="tex-font-style-bf">Antihype</span>. It has the following rules:</p><ol> <li> You can join the pyramid for free and get $0$ coins. </li><li> If you are already a member of Antihype, you can invite your friend who is currently not a member of Antihype, and get a number of coins equal to your age (for each friend you invite). </li></ol><p>$n$ people have heard about Antihype recently, the $i$-th person's age is $a_i$. Some of them are friends, but friendship is a weird thing now: the $i$-th person is a friend of the $j$-th person <span class="tex-font-style-bf">if and only if</span> $a_i \text{ AND } a_j = 0$, where $\text{AND}$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#AND">bitwise AND operation</a>.</p><p>Nobody among the $n$ people is a member of Antihype at the moment. They want to cooperate to join and invite each other to Antihype in a way that maximizes their combined gainings. Could you help them? </p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1\le n \le 2\cdot 10^5$) &nbsp;— the number of people.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0\le a_i \le 2\cdot 10^5$) &nbsp;— the ages of the people.</p></div><div class="output-specification"><p>Output exactly one integer &nbsp;— the maximum possible combined gainings of all $n$ people.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1\le n \le 2\cdot 10^5$) &nbsp;— the number of people.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0\le a_i \le 2\cdot 10^5$) &nbsp;— the ages of the people.</p>

## Output

<p>Output exactly one integer &nbsp;— the maximum possible combined gainings of all $n$ people.</p>





```input1
3
1 2 3
```




```output1
2
```



## Note

<p>Only the first and second persons are friends. The second can join Antihype and invite the first one, getting $2$ for it.</p>
