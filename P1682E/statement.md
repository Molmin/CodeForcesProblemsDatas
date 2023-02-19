## Description

<div><p>Alice had a permutation $p$ of numbers from $1$ to $n$. Alice can swap a pair $(x, y)$ which means swapping elements at positions $x$ and $y$ in $p$ (i.e. swap $p_x$ and $p_y$). Alice recently learned her first sorting algorithm, so she decided to sort her permutation in the <span class="tex-font-style-bf">minimum</span> number of swaps possible. She wrote down all the swaps in the order in which she performed them to sort the permutation on a piece of paper. </p><p>For example,</p><ul> <li> $[(2, 3), (1, 3)]$ is a valid swap sequence by Alice for permutation $p = [3, 1, 2]$ whereas $[(1, 3), (2, 3)]$ is not because it doesn't sort the permutation. Note that we cannot sort the permutation in less than $2$ swaps. </li><li> $[(1, 2), (2, 3), (2, 4), (2, 3)]$ cannot be a sequence of swaps by Alice for $p = [2, 1, 4, 3]$ even if it sorts the permutation because $p$ can be sorted in $2$ swaps, for example using the sequence $[(4, 3), (1, 2)]$. </li></ul><p>Unfortunately, Bob shuffled the sequence of swaps written by Alice.</p><p>You are given Alice's permutation $p$ and the swaps performed by Alice in arbitrary order. Can you restore the correct sequence of swaps that sorts the permutation $p$? Since Alice wrote correct swaps before Bob shuffled them up, it is guaranteed that there exists some order of swaps that sorts the permutation.</p></div><div class="input-specification"><p>The first line contains $2$ integers $n$ and $m$ $(2 \le n \le 2 \cdot 10^5, 1 \le m \le n - 1)$ &nbsp;— the size of permutation and the minimum number of swaps required to sort the permutation.</p><p>The next line contains $n$ integers $p_1, p_2, ..., p_n$ ($1 \le p_i \le n$, all $p_i$ are distinct) &nbsp;— the elements of $p$. It is guaranteed that $p$ forms a permutation.</p><p>Then $m$ lines follow. The $i$-th of the next $m$ lines contains two integers $x_i$ and $y_i$ &nbsp;— the $i$-th swap $(x_i, y_i)$.</p><p>It is guaranteed that it is possible to sort $p$ with these $m$ swaps and that there is no way to sort $p$ with less than $m$ swaps.</p></div><div class="output-specification"><p>Print a permutation of $m$ integers &nbsp;— a valid order of swaps written by Alice that sorts the permutation $p$. See sample explanation for better understanding.</p><p>In case of multiple possible answers, output any.</p></div>

## Input

<p>The first line contains $2$ integers $n$ and $m$ $(2 \le n \le 2 \cdot 10^5, 1 \le m \le n - 1)$ &nbsp;— the size of permutation and the minimum number of swaps required to sort the permutation.</p><p>The next line contains $n$ integers $p_1, p_2, ..., p_n$ ($1 \le p_i \le n$, all $p_i$ are distinct) &nbsp;— the elements of $p$. It is guaranteed that $p$ forms a permutation.</p><p>Then $m$ lines follow. The $i$-th of the next $m$ lines contains two integers $x_i$ and $y_i$ &nbsp;— the $i$-th swap $(x_i, y_i)$.</p><p>It is guaranteed that it is possible to sort $p$ with these $m$ swaps and that there is no way to sort $p$ with less than $m$ swaps.</p>

## Output

<p>Print a permutation of $m$ integers &nbsp;— a valid order of swaps written by Alice that sorts the permutation $p$. See sample explanation for better understanding.</p><p>In case of multiple possible answers, output any.</p>





```input1
4 3
2 3 4 1
1 4
2 1
1 3
```




```input2
6 4
6 5 1 3 2 4
3 1
2 5
6 3
6 4
```




```output1
2 3 1
```




```output2
4 1 3 2
```



## Note

<p>In the first example, $p = [2, 3, 4, 1]$, $m = 3$ and given swaps are $[(1, 4), (2, 1), (1, 3)]$.</p><p>There is only one correct order of swaps i.e $[2, 3, 1]$.</p><ol> <li> First we perform the swap $2$ from the input i.e $(2, 1)$, $p$ becomes $[3, 2, 4, 1]$. </li><li> Then we perform the swap $3$ from the input i.e $(1, 3)$, $p$ becomes $[4, 2, 3, 1]$. </li><li> Finally we perform the swap $1$ from the input i.e $(1, 4)$ and $p$ becomes $[1, 2, 3, 4]$ which is sorted. </li></ol><p>In the second example, $p = [6, 5, 1, 3, 2, 4]$, $m = 4$ and the given swaps are $[(3, 1), (2, 5), (6, 3), (6, 4)]$.</p><p>One possible correct order of swaps is $[4, 2, 1, 3]$.</p><ol> <li> Perform the swap $4$ from the input i.e $(6, 4)$, $p$ becomes $[6, 5, 1, 4, 2, 3]$. </li><li> Perform the swap $2$ from the input i.e $(2, 5)$, $p$ becomes $[6, 2, 1, 4, 5, 3]$. </li><li> Perform the swap $1$ from the input i.e $(3, 1)$, $p$ becomes $[1, 2, 6, 4, 5, 3]$. </li><li> Perform the swap $3$ from the input i.e $(6, 3)$ and $p$ becomes $[1, 2, 3, 4, 5, 6]$ which is sorted. </li></ol><p>There can be other possible answers such as $[1, 2, 4, 3]$.</p>
