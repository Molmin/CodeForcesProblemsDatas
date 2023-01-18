## Description

<div><p>You have to restore the wall. The wall consists of $N$ pillars of bricks, the height of the $i$-th pillar is initially equal to $h_{i}$, the height is measured in number of bricks. After the restoration all the $N$ pillars should have equal heights.</p><p>You are allowed the following operations:</p><ul><li> put a brick on top of one pillar, the cost of this operation is $A$;</li><li> remove a brick from the top of one non-empty pillar, the cost of this operation is $R$;</li><li> move a brick from the top of one non-empty pillar to the top of another pillar, the cost of this operation is $M$.</li></ul><p>You cannot create additional pillars or ignore some of pre-existing pillars even if their height becomes $0$.</p><p>What is the minimal total cost of restoration, in other words, what is the minimal total cost to make all the pillars of equal height?</p></div><div class="input-specification"><p>The first line of input contains four integers $N$, $A$, $R$, $M$ ($1 \le N \le 10^{5}$, $0 \le A, R, M \le 10^{4}$)&nbsp;— the number of pillars and the costs of operations.</p><p>The second line contains $N$ integers $h_{i}$ ($0 \le h_{i} \le 10^{9}$)&nbsp;— initial heights of pillars.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the minimal cost of restoration.</p></div>

## Input

<p>The first line of input contains four integers $N$, $A$, $R$, $M$ ($1 \le N \le 10^{5}$, $0 \le A, R, M \le 10^{4}$)&nbsp;— the number of pillars and the costs of operations.</p><p>The second line contains $N$ integers $h_{i}$ ($0 \le h_{i} \le 10^{9}$)&nbsp;— initial heights of pillars.</p>

## Output

<p>Print one integer&nbsp;— the minimal cost of restoration.</p>





```input1
3 1 100 100
1 3 8
```




```input2
3 100 1 100
1 3 8
```




```input3
3 100 100 1
1 3 8
```




```input4
5 1 2 4
5 5 3 6 5
```




```input5
5 1 2 2
5 5 3 6 5
```




```output1
12
```




```output2
9
```




```output3
4
```




```output4
4
```




```output5
3
```


