## Description

<div><p>Maksim has $n$ objects and $m$ boxes, each box has size exactly $k$. Objects are numbered from $1$ to $n$ in order from left to right, the size of the $i$-th object is $a_i$.</p><p>Maksim wants to pack his objects into the boxes and he will pack objects by the following algorithm: he takes one of the empty boxes he has, goes from left to right through the objects, and if the $i$-th object fits in the current box (the remaining size of the box is greater than or equal to $a_i$), he puts it in the box, and the remaining size of the box decreases by $a_i$. Otherwise he takes the new empty box and continues the process above. If he has no empty boxes and there is at least one object not in some box then Maksim cannot pack the chosen set of objects.</p><p>Maksim wants to know the maximum number of objects he can pack by the algorithm above. To reach this target, <span class="tex-font-style-bf">he will throw out the leftmost object from the set until the remaining set of objects can be packed in boxes he has</span>. Your task is to say the maximum number of objects Maksim can pack in boxes he has.</p><p>Each time when Maksim tries to pack the objects into the boxes, he will make empty all the boxes he has before do it (and the relative order of the remaining set of objects will not change).</p></div><div class="input-specification"><p>The first line of the input contains three integers $n$, $m$, $k$ ($1 \le n, m \le 2 \cdot 10^5$, $1 \le k \le 10^9$) — the number of objects, the number of boxes and the size of each box.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le k$), where $a_i$ is the size of the $i$-th object.</p></div><div class="output-specification"><p>Print the maximum number of objects Maksim can pack using the algorithm described in the problem statement.</p></div>

## Input

<p>The first line of the input contains three integers $n$, $m$, $k$ ($1 \le n, m \le 2 \cdot 10^5$, $1 \le k \le 10^9$) — the number of objects, the number of boxes and the size of each box.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le k$), where $a_i$ is the size of the $i$-th object.</p>

## Output

<p>Print the maximum number of objects Maksim can pack using the algorithm described in the problem statement.</p>





```input1
5 2 6
5 2 1 4 2

```




```input2
5 1 4
4 2 3 4 1

```




```input3
5 3 3
1 2 3 1 1

```




```output1
4

```




```output2
1

```




```output3
5

```



## Note

<p>In the first example Maksim can pack only $4$ objects. Firstly, he tries to pack all the $5$ objects. Distribution of objects will be $[5], [2, 1]$. Maxim cannot pack the next object in the second box and he has no more empty boxes at all. Next he will throw out the first object and the objects distribution will be $[2, 1], [4, 2]$. So the answer is $4$.</p><p>In the second example it is obvious that Maksim cannot pack all the objects starting from first, second, third and fourth (in all these cases the distribution of objects is $[4]$), but he can pack the last object ($[1]$).</p><p>In the third example Maksim can pack all the objects he has. The distribution will be $[1, 2], [3], [1, 1]$.</p>
