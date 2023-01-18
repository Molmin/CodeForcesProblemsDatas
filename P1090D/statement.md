## Description

<div><p>Vasya had an array of $n$ integers, each element of the array was from $1$ to $n$. He chose $m$ pairs of different positions and wrote them down to a sheet of paper. Then Vasya compared the elements at these positions, and wrote down the results of the comparisons to another sheet of paper. For each pair he wrote either "greater", "less", or "equal".</p><p>After several years, he has found the first sheet of paper, but he couldn't find the second one. Also he doesn't remember the array he had. In particular, he doesn't remember if the array had equal elements. He has told this sad story to his informatics teacher Dr Helen.</p><p>She told him that it could be the case that even if Vasya finds his second sheet, he would still not be able to find out whether the array had two equal elements. </p><p>Now Vasya wants to find two arrays of integers, each of length $n$. All elements of the first array must be distinct, and there must be two equal elements in the second array. For each pair of positions Vasya wrote at the first sheet of paper, the result of the comparison must be the same for the corresponding elements of the first array, and the corresponding elements of the second array. </p><p>Help Vasya find two such arrays of length $n$, or find out that there are no such arrays for his sets of pairs.</p></div><div class="input-specification"><p>The first line of input contains two integers $n$, $m$&nbsp;— the number of elements in the array and number of comparisons made by Vasya ($1 \le n \le 100\,000$, $0 \le m \le 100\,000$).</p><p>Each of the following $m$ lines contains two integers $a_i$, $b_i$ &nbsp;— the positions of the $i$-th comparison ($1 \le a_i, b_i \le n$; $a_i \ne b_i$). It's guaranteed that any unordered pair is given in the input at most once.</p></div><div class="output-specification"><p>The first line of output must contain "<span class="tex-font-style-tt">YES</span>" if there exist two arrays, such that the results of comparisons would be the same, and all numbers in the first one are distinct, and the second one contains two equal numbers. Otherwise it must contain "<span class="tex-font-style-tt">NO</span>".</p><p>If the arrays exist, the second line must contain the array of distinct integers, the third line must contain the array, that contains at least one pair of equal elements. Elements of the arrays must be integers from $1$ to $n$.</p></div>

## Input

<p>The first line of input contains two integers $n$, $m$&nbsp;— the number of elements in the array and number of comparisons made by Vasya ($1 \le n \le 100\,000$, $0 \le m \le 100\,000$).</p><p>Each of the following $m$ lines contains two integers $a_i$, $b_i$ &nbsp;— the positions of the $i$-th comparison ($1 \le a_i, b_i \le n$; $a_i \ne b_i$). It's guaranteed that any unordered pair is given in the input at most once.</p>

## Output

<p>The first line of output must contain "<span class="tex-font-style-tt">YES</span>" if there exist two arrays, such that the results of comparisons would be the same, and all numbers in the first one are distinct, and the second one contains two equal numbers. Otherwise it must contain "<span class="tex-font-style-tt">NO</span>".</p><p>If the arrays exist, the second line must contain the array of distinct integers, the third line must contain the array, that contains at least one pair of equal elements. Elements of the arrays must be integers from $1$ to $n$.</p>





```input1
1 0
```




```input2
3 1
1 2
```




```input3
4 3
1 2
1 3
2 4
```




```output1
NO
```




```output2
YES
1 3 2 
1 3 1
```




```output3
YES
1 3 4 2 
1 3 4 1
```


