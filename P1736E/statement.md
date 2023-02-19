## Description

<div><p>You're given an array consisting of $n$ integers. You have to perform $n$ turns.</p><p>Initially your score is $0$.</p><p>On the $i$-th turn, you are allowed to leave the array as it is or swap any one pair of $2$ adjacent elements in the array and change exactly one of them to $0$(and leave the value of other element unchanged) after swapping. In either case(whether you swap or not), after this you add $a_i$ to your score. </p><p>What's the maximum possible score you can get?</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 500$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^6$).</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the maximum possible score.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 500$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^6$).</p>

## Output

<p>Print a single integer&nbsp;— the maximum possible score.</p>





```input1
2
3 1
```




```input2
5
7 3 9 6 12
```




```output1
6
```




```output2
52
```



## Note

<p>In the first example, to get the maximum score we do as follows. Do nothing on the first turn, add $3$ to the score. Swap the first and the second elements and turn $1$ to $0$ on the second turn, and add $3$ to the score. The final score is $6$.</p>
