## Description

<div><p>Three little pigs from all over the world are meeting for a convention! Every minute, a triple of 3 new pigs arrives on the convention floor. After the $n$-th minute, the convention ends.</p><p>The big bad wolf has learned about this convention, and he has an attack plan. At some minute in the convention, he will arrive and eat exactly $x$ pigs. Then he will get away.</p><p>The wolf wants Gregor to help him figure out the number of possible attack plans that involve eating exactly $x$ pigs for various values of $x$ ($1 \le x \le 3n$). Two attack plans are considered different, if they occur at different times or if the sets of little pigs to eat are different.</p><p>Note that all queries are independent, that is, the wolf does not eat the little pigs, he only makes plans!</p></div><div class="input-specification"><p>The first line of input contains two integers $n$ and $q$ ($1 \le n \le 10^6$, $1 \le q \le 2\cdot 10^5$), the number of minutes the convention lasts and the number of queries the wolf asks.</p><p>Each of the next $q$ lines contains a single integer $x_i$ ($1 \le x_i \le 3n$), the number of pigs the wolf will eat in the $i$-th query.</p></div><div class="output-specification"><p>You should print $q$ lines, with line $i$ representing the number of attack plans if the wolf wants to eat $x_i$ pigs. Since each query answer can be large, output each answer modulo $10^9+7$.</p></div>

## Input

<p>The first line of input contains two integers $n$ and $q$ ($1 \le n \le 10^6$, $1 \le q \le 2\cdot 10^5$), the number of minutes the convention lasts and the number of queries the wolf asks.</p><p>Each of the next $q$ lines contains a single integer $x_i$ ($1 \le x_i \le 3n$), the number of pigs the wolf will eat in the $i$-th query.</p>

## Output

<p>You should print $q$ lines, with line $i$ representing the number of attack plans if the wolf wants to eat $x_i$ pigs. Since each query answer can be large, output each answer modulo $10^9+7$.</p>





```input1
2 3
1
5
6
```




```input2
5 4
2
4
6
8
```




```output1
9
6
1
```




```output2
225
2001
6014
6939
```



## Note

<p>In the example test, $n=2$. Thus, there are $3$ pigs at minute $1$, and $6$ pigs at minute $2$. There are three queries: $x=1$, $x=5$, and $x=6$.</p><p>If the wolf wants to eat $1$ pig, he can do so in $3+6=9$ possible attack plans, depending on whether he arrives at minute $1$ or $2$.</p><p>If the wolf wants to eat $5$ pigs, the wolf cannot arrive at minute $1$, since there aren't enough pigs at that time. Therefore, the wolf has to arrive at minute $2$, and there are $6$ possible attack plans.</p><p>If the wolf wants to eat $6$ pigs, his only plan is to arrive at the end of the convention and devour everybody.</p><p>Remember to output your answers modulo $10^9+7$!</p>
