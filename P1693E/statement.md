## Description

<div><p>Yeri has an array of $n + 2$ non-negative integers : $a_0, a_1, ..., a_n, a_{n + 1}$.</p><p>We know that $a_0 = a_{n + 1} = 0$.</p><p>She wants to make all the elements of $a$ equal to zero in the minimum number of operations.</p><p>In one operation she can do one of the following: </p><ul><li> Choose the leftmost maximum element and change it to the maximum of the elements on its left.</li><li> Choose the rightmost maximum element and change it to the maximum of the elements on its right.</li></ul><p>Help her find the minimum number of operations needed to make all elements of $a$ equal to zero.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le n$).</p></div><div class="output-specification"><p>Print a single integer &nbsp;— the minimum number of operations needed to make all elements of $a$ equal to zero.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le n$).</p>

## Output

<p>Print a single integer &nbsp;— the minimum number of operations needed to make all elements of $a$ equal to zero.</p>





```input1
6
1 4 2 4 0 2
```




```input2
5
1 3 5 4 2
```




```input3
4
0 0 0 0
```




```output1
7
```




```output2
9
```




```output3
0
```



## Note

<p>In the first sample, you get $\langle 1, \underline{1}, 2, 4, 0, 2 \rangle$ by performing the first operation and $\langle 1, 4, 2, \underline{2}, 0, 2 \rangle$ by performing the second operation.</p><p>One way to achieve our goal is shown below. (The underlines show the last change.) $\langle 1, 4, 2, 4, 0, 2 \rangle \to \langle 1, 4, 2, \underline{2}, 0, 2 \rangle \to \langle 1, \underline{1}, 2, 2, 0, 2 \rangle \to \langle 1, 1, 2, 2, 0, \underline{0} \rangle \to \langle 1, 1, 2, \underline{0}, 0, 0 \rangle \to \langle 1, 1, \underline{0}, 0, 0, 0 \rangle \to \langle \underline{0}, 1, 0, 0, 0, 0 \rangle \to \langle 0, \underline{0}, 0, 0, 0, 0 \rangle $</p><p>In the third sample each element is already equal to zero so no operations are needed.</p>
