## Description

<div><p><span class="tex-font-style-bf">This is the easy version of the problem. The only difference between the two versions is the constraint on $n$ and $x$. You can make hacks only if both versions of the problem are solved.</span></p><p>Little09 has been interested in magic for a long time, and it's so lucky that he meets a magician! The magician will perform $n$ operations, each of them is one of the following three:</p><ul><li> $1\ x$: Create a pig with $x$ Health Points. </li><li> $2\ x$: Reduce the Health Point of all living pigs by $x$. </li><li> $3$: Repeat all previous operations. Formally, assuming that this is the $i$-th operation in the operation sequence, perform the first $i-1$ operations (including "Repeat" operations involved) in turn.</li></ul><p>A pig will die when its Health Point is less than or equal to $0$. </p><p>Little09 wants to know how many living pigs there are after all the operations. Please, print the answer modulo $998\,244\,353$.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1\leq n\leq 2\cdot 10^5$) &nbsp;— the number of operations.</p><p>Each of the following $n$ lines contains an operation given in the form described in the problem statement. It's guaranteed that $1\leq x\leq 2\cdot 10^5$ in operations of the first two types.</p></div><div class="output-specification"><p>Print a single integer &nbsp;— the number of living pigs after all the operations, modulo $998\,244\,353$.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1\leq n\leq 2\cdot 10^5$) &nbsp;— the number of operations.</p><p>Each of the following $n$ lines contains an operation given in the form described in the problem statement. It's guaranteed that $1\leq x\leq 2\cdot 10^5$ in operations of the first two types.</p>

## Output

<p>Print a single integer &nbsp;— the number of living pigs after all the operations, modulo $998\,244\,353$.</p>





```input1
4
1 8
2 3
3
3
```




```input2
6
1 5
1 6
2 2
3
1 4
3
```




```input3
12
2 1
1 15
1 9
3
1 12
2 2
1 13
3
2 1
1 9
1 8
3
```




```output1
2
```




```output2
5
```




```output3
17
```



## Note

<p>In the first example, the operations are equivalent to repeating four times: create a pig with $8$ Health Points and then reduce the Health Points of all living pigs by $3$. It is easy to find that there are two living pigs in the end with $2$ and $5$ Health Points.</p>
