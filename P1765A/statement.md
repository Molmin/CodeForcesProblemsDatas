## Description

<div><p>BerSoft is the biggest IT corporation in Berland, and Monocarp is the head of its security department. This time, he faced the most difficult task ever. </p><p>Basically, there are $n$ developers working at BerSoft, numbered from $1$ to $n$. There are $m$ documents shared on the internal network, numbered from $1$ to $m$. There is a table of access requirements $a$ such that $a_{i,j}$ (the $j$-th element of the $i$-th row) is $1$ if the $i$-th developer should have access to the $j$-th document, and $0$ if they should have no access to it.</p><p>In order to restrict the access, Monocarp is going to perform the following actions: </p><ul> <li> choose the number of access groups $k \ge 1$; </li><li> assign each document an access group (an integer from $1$ to $k$) and the required access level (an integer from $1$ to $10^9$); </li><li> assign each developer $k$ integer values (from $1$ to $10^9$)&nbsp;— their access levels for each of the access groups. </li></ul><p>The developer $i$ has access to the document $j$ if their access level for the access group of the document is greater than or equal to the required access level of the document.</p><p>What's the smallest number of access groups Monocarp can choose so that it's possible to assign access groups and access levels in order to satisfy the table of access requirements?</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 500$)&nbsp;— the number of developers and the number of documents.</p><p>Each of the next $n$ lines contains a binary string of length $m$&nbsp;— the table of access requirements. The $j$-th element of the $i$-th row is $1$ if the $i$-th developer should have access to the $j$-th document, and $0$ if they should have no access to it.</p></div><div class="output-specification"><p>The first line should contain a single integer $k$&nbsp;— the smallest number of access groups Monocarp can choose so that it's possible to assign access groups and access levels in order to satisfy the table of access requirements.</p><p>The second line should contain $m$ integers from $1$ to $k$&nbsp;— the access groups of the documents.</p><p>The third line should contain $m$ integers from $1$ to $10^9$&nbsp;— the required access levels of the documents.</p><p>The $i$-th of the next $n$ lines should contain $k$ integers from $1$ to $10^9$&nbsp;— the access level of the $i$-th developer on each of the access groups.</p><p>If there are multiple solutions, print any of them.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 500$)&nbsp;— the number of developers and the number of documents.</p><p>Each of the next $n$ lines contains a binary string of length $m$&nbsp;— the table of access requirements. The $j$-th element of the $i$-th row is $1$ if the $i$-th developer should have access to the $j$-th document, and $0$ if they should have no access to it.</p>

## Output

<p>The first line should contain a single integer $k$&nbsp;— the smallest number of access groups Monocarp can choose so that it's possible to assign access groups and access levels in order to satisfy the table of access requirements.</p><p>The second line should contain $m$ integers from $1$ to $k$&nbsp;— the access groups of the documents.</p><p>The third line should contain $m$ integers from $1$ to $10^9$&nbsp;— the required access levels of the documents.</p><p>The $i$-th of the next $n$ lines should contain $k$ integers from $1$ to $10^9$&nbsp;— the access level of the $i$-th developer on each of the access groups.</p><p>If there are multiple solutions, print any of them.</p>





```input1
3 2
01
11
10
```




```input2
2 3
101
100
```




```output1
2
1 2 
2 2 
1 2 
2 2 
2 1
```




```output2
1
1 1 1
1 10 5
8
3
```



## Note

<p>In the first example, we assign the documents to different access groups. Both documents have level $2$ in their access group. This way, we can assign the developers, who need the access, level $2$, and the developers, who have to have no access, level $1$.</p><p>If they had the same access group, it would be impossible to assign access levels to developers $1$ and $3$. Developer $1$ should've had a lower level than developer $3$ in this group to not be able to access document $1$. At the same time, developer $3$ should've had a lower level than developer $1$ in this group to not be able to access document $2$. Since they can't both have lower level than each other, it's impossible to have only one access group.</p><p>In the second example, it's possible to assign all documents to the same access group. </p>
