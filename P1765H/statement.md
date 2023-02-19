## Description

<div><p>There are $n$ people (numbered from $1$ to $n$) signed up for a doctor's appointment. The doctor has to choose in which order he will appoint these people. The $i$-th patient should be appointed among the first $p_i$ people. There are also $m$ restrictions of the following format: the $i$-th restriction is denoted by two integers $(a_i, b_i)$ and means that the patient with the index $a_i$ should be appointed earlier than the patient with the index $b_i$.</p><p>For example, if $n = 4$, $p = [2, 3, 2, 4]$, $m = 1$, $a = [3]$ and $b = [1]$, then the only order of appointment of patients that does not violate the restrictions is $[3, 1, 2, 4]$. For $n =3$, $p = [3, 3, 3]$, $m = 0$, $a = []$ and $b = []$, any order of appointment is valid.</p><p>For each patient, calculate the minimum position in the order that they can have among all possible orderings that don't violate the restrictions.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n \le 2000$; $0 \le m \le 2000$).</p><p>The second line contains $n$ integers $p_1, p_2, \dots, p_n$ ($1 \le p_i \le n$).</p><p>Then $m$ lines follow. The $i$-th of them contains two integers $a_i$ and $b_i$ ($1 \le a_i, b_i \le n$; $a_i \ne b_i$). All pairs of $(a_i, b_i)$ are distinct (i. e. if $i \ne j$, then either $a_i \ne a_j$, $b_i \ne b_j$, or both).</p><p>Additional constraint on the input: there is at least one valid order of patients.</p></div><div class="output-specification"><p>Print $n$ integers, where $i$-th integer is equal to the minimum position of $i$-th patient in the order, among all valid orders. Positions in the order are numbered from $1$ to $n$.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n \le 2000$; $0 \le m \le 2000$).</p><p>The second line contains $n$ integers $p_1, p_2, \dots, p_n$ ($1 \le p_i \le n$).</p><p>Then $m$ lines follow. The $i$-th of them contains two integers $a_i$ and $b_i$ ($1 \le a_i, b_i \le n$; $a_i \ne b_i$). All pairs of $(a_i, b_i)$ are distinct (i. e. if $i \ne j$, then either $a_i \ne a_j$, $b_i \ne b_j$, or both).</p><p>Additional constraint on the input: there is at least one valid order of patients.</p>

## Output

<p>Print $n$ integers, where $i$-th integer is equal to the minimum position of $i$-th patient in the order, among all valid orders. Positions in the order are numbered from $1$ to $n$.</p>





```input1
4 1
2 3 2 4
3 1
```




```input2
3 0
3 3 3
```




```input3
5 3
4 3 3 2 5
3 1
1 5
4 2
```




```output1
2 3 1 4
```




```output2
1 1 1
```




```output3
4 2 1 1 5
```



## Note

<p>In the first example, $[3, 1, 2, 4]$ the only one valid order, so the minimum position of each patient is equal to their position in this order.</p><p>In the second example, any order is valid, so any patient can be appointed first.</p><p>In the third example, there are three valid orders: $[4, 2, 3, 1, 5]$, $[3, 4, 2, 1, 5]$ and $[4, 3, 2, 1, 5]$.</p>
