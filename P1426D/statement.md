## Description

<div><p>Kolya got an integer array $a_1, a_2, \dots, a_n$. The array can contain both positive and negative integers, but Kolya doesn't like $0$, so the array doesn't contain any zeros.</p><p>Kolya doesn't like that the sum of some subsegments of his array can be $0$. The subsegment is some consecutive segment of elements of the array. </p><p>You have to help Kolya and change his array in such a way that it doesn't contain any subsegments with the sum $0$. To reach this goal, you can insert any integers between any pair of adjacent elements of the array (integers can be really any: positive, negative, $0$, any by absolute value, even such a huge that they can't be represented in most standard programming languages).</p><p>Your task is to find the minimum number of integers you have to insert into Kolya's array in such a way that the resulting array doesn't contain any subsegments with the sum $0$.</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($2 \le n \le 200\,000$) — the number of elements in Kolya's array.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($-10^{9} \le a_i \le 10^{9}, a_i \neq 0$) — the description of Kolya's array.</p></div><div class="output-specification"><p>Print the minimum number of integers you have to insert into Kolya's array in such a way that the resulting array doesn't contain any subsegments with the sum $0$.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($2 \le n \le 200\,000$) — the number of elements in Kolya's array.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($-10^{9} \le a_i \le 10^{9}, a_i \neq 0$) — the description of Kolya's array.</p>

## Output

<p>Print the minimum number of integers you have to insert into Kolya's array in such a way that the resulting array doesn't contain any subsegments with the sum $0$.</p>





```input1
4
1 -5 3 2
```




```input2
5
4 -2 3 -9 2
```




```input3
9
-1 1 -1 1 -1 1 1 -1 -1
```




```input4
8
16 -5 -11 -15 10 5 4 -4
```




```output1
1
```




```output2
0
```




```output3
6
```




```output4
3
```



## Note

<p>Consider the first example. There is only one subsegment with the sum $0$. It starts in the second element and ends in the fourth element. It's enough to insert one element so the array doesn't contain any subsegments with the sum equal to zero. For example, it is possible to insert the integer $1$ between second and third elements of the array.</p><p>There are no subsegments having sum $0$ in the second example so you don't need to do anything.</p>
