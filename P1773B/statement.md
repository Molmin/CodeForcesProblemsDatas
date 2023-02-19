## Description

<div><p>There are $n$ employees in the BinCoin company numbered from $1$ to $n$. The subordination structure in this company is a rooted tree. In other words: </p><ul> <li> There is one CEO in the company&nbsp;— the main boss. </li><li> Each other employee has exactly one direct superior. </li><li> There are no cycles in the subordination structure. </li></ul><p>Moreover, due to the inexplicable love of the CEO of BinCoin for all the binary stuff, the subordination structure in the company is a <span class="tex-font-style-bf">binary</span> rooted tree. That means each employee is directly superior to exactly zero or two other employees.</p><p>In the CEO's opinion, working in this company is almost as dangerous as in mines. So, employees should sign the waiver of claims sometimes. This process happens in the following way. Initially, CEO takes the journal, then recursively the following procedure is performed:</p><ul> <li> If an employee that holds the journal does not have any subordinates, they sign the waiver in the journal and give it back to their superior. The procedure stops if that was the CEO, who has no superior. </li><li> Otherwise <ul> <li> they choose one of two of their direct subordinates uniformly at random and give the journal to one of them; </li><li> when they get the journal back, they sign it; </li><li> and then they give it to another direct subordinate; </li><li> when they get it back again, they give it back to their superior. The procedure stops if that was the CEO, who has no superior. </li></ul> </li></ul><p>All random choices are independent.</p><p>One day, the CEO realized that they could not remember the subordination tree. Fortunately, they have the journal with $k$ records. Each record is a sequence of employees in the order they've signed in a journal.</p><p>Help CEO restore the subordination tree.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$&nbsp;— the number of employees and the number of records in the journal ($1 \le n \le 999$; $50 \le k \le 100$).</p><p>Each of the next $k$ lines contains a permutation of integers from $1$ to $n$&nbsp;— the order of employees in the corresponding record.</p><p>It is guaranteed that the input was obtained as described in the statement with a real random choice.</p></div><div class="output-specification"><p>Output $n$ integers $p_i$. If $i$ is a CEO, then $p_i$ should be $-1$. Otherwise, $p_i$ should be the index of the direct superior of $i$-th employee.</p><p>Your output should correspond to a binary rooted tree. If there are several trees satisfying the input, you can output any one of them.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$&nbsp;— the number of employees and the number of records in the journal ($1 \le n \le 999$; $50 \le k \le 100$).</p><p>Each of the next $k$ lines contains a permutation of integers from $1$ to $n$&nbsp;— the order of employees in the corresponding record.</p><p>It is guaranteed that the input was obtained as described in the statement with a real random choice.</p>

## Output

<p>Output $n$ integers $p_i$. If $i$ is a CEO, then $p_i$ should be $-1$. Otherwise, $p_i$ should be the index of the direct superior of $i$-th employee.</p><p>Your output should correspond to a binary rooted tree. If there are several trees satisfying the input, you can output any one of them.</p>





```input1
3 50
1 2 3    1 2 3    3 2 1    1 2 3
3 2 1    1 2 3    1 2 3    1 2 3
1 2 3    3 2 1    1 2 3    3 2 1
1 2 3    3 2 1    1 2 3    3 2 1
1 2 3    1 2 3    3 2 1    1 2 3
3 2 1    1 2 3    3 2 1    1 2 3
1 2 3    3 2 1    1 2 3    1 2 3
1 2 3    1 2 3    3 2 1    1 2 3
3 2 1    3 2 1    1 2 3    3 2 1
1 2 3    3 2 1    3 2 1    1 2 3
1 2 3    3 2 1    1 2 3    3 2 1
3 2 1    3 2 1    1 2 3    1 2 3
3 2 1    3 2 1
```




```input2
5 60
2 4 3 5 1    1 5 2 4 3    1 5 2 4 3
1 5 2 4 3    1 5 3 4 2    1 5 3 4 2
1 5 3 4 2    1 5 3 4 2    1 5 3 4 2
3 4 2 5 1    2 4 3 5 1    1 5 2 4 3
3 4 2 5 1    2 4 3 5 1    2 4 3 5 1
1 5 2 4 3    3 4 2 5 1    3 4 2 5 1
1 5 2 4 3    2 4 3 5 1    1 5 2 4 3
1 5 3 4 2    3 4 2 5 1    1 5 3 4 2
1 5 2 4 3    1 5 3 4 2    1 5 2 4 3
2 4 3 5 1    2 4 3 5 1    2 4 3 5 1
2 4 3 5 1    2 4 3 5 1    1 5 2 4 3
1 5 3 4 2    1 5 2 4 3    3 4 2 5 1
1 5 3 4 2    3 4 2 5 1    3 4 2 5 1
1 5 2 4 3    2 4 3 5 1    1 5 2 4 3
1 5 3 4 2    2 4 3 5 1    2 4 3 5 1
1 5 2 4 3    1 5 2 4 3    1 5 2 4 3
1 5 2 4 3    1 5 2 4 3    3 4 2 5 1
3 4 2 5 1    3 4 2 5 1    1 5 2 4 3
1 5 3 4 2    1 5 3 4 2    2 4 3 5 1
3 4 2 5 1    1 5 2 4 3    3 4 2 5 1
```




```output1
2 -1 2
```




```output2
5 4 4 5 -1
```



## Note

<p>In order to fit on the page, several consecutive lines in the examples were joined into one. The real inputs follow the input description.</p>
