## Description

<div><p>Imagine that there is a group of three friends: A, B and С. A owes B 20 rubles and B owes C 20 rubles. The total sum of the debts is 40 rubles. You can see that the debts are not organized in a very optimal manner. Let's rearrange them like that: assume that A owes C 20 rubles and B doesn't owe anything to anybody. The debts still mean the same but the total sum of the debts now equals 20 rubles.</p><p>This task is a generalisation of a described example. Imagine that your group of friends has <span class="tex-span"><i>n</i></span> people and you know the debts between the people. Optimize the given debts without changing their meaning. In other words, finally for each friend the difference between the total money he should give and the total money he should take must be the same. Print the minimum sum of all debts in the optimal rearrangement of the debts. See the notes to the test samples to better understand the problem.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100;&nbsp;0 ≤ <i>m</i> ≤ 10<sup class="upper-index">4</sup>)</span>. The next <span class="tex-span"><i>m</i></span> lines contain the debts. The <span class="tex-span"><i>i</i></span>-th line contains three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>;&nbsp;1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span>, which mean that person <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> owes person <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> rubles.</p><p>Assume that the people are numbered by integers from 1 to <span class="tex-span"><i>n</i></span>.</p><p>It is guaranteed that the same pair of people occurs at most once in the input. The input doesn't simultaneously contain pair of people <span class="tex-span">(<i>x</i>, <i>y</i>)</span> and pair of people <span class="tex-span">(<i>y</i>, <i>x</i>)</span>.</p></div><div class="output-specification"><p>Print a single integer — the minimum sum of debts in the optimal rearrangement.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100;&nbsp;0 ≤ <i>m</i> ≤ 10<sup class="upper-index">4</sup>)</span>. The next <span class="tex-span"><i>m</i></span> lines contain the debts. The <span class="tex-span"><i>i</i></span>-th line contains three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>;&nbsp;1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span>, which mean that person <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> owes person <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> rubles.</p><p>Assume that the people are numbered by integers from 1 to <span class="tex-span"><i>n</i></span>.</p><p>It is guaranteed that the same pair of people occurs at most once in the input. The input doesn't simultaneously contain pair of people <span class="tex-span">(<i>x</i>, <i>y</i>)</span> and pair of people <span class="tex-span">(<i>y</i>, <i>x</i>)</span>.</p>

## Output

<p>Print a single integer — the minimum sum of debts in the optimal rearrangement.</p>





```input1
5 3
1 2 10
2 3 1
2 4 1

```




```input2
3 0

```




```input3
4 3
1 2 1
2 3 1
3 1 1

```




```output1
10

```




```output2
0

```




```output3
0

```



## Note

<p>In the first sample, you can assume that person number 1 owes 8 rubles to person number 2, 1 ruble to person number 3 and 1 ruble to person number 4. He doesn't owe anybody else anything. In the end, the total debt equals 10.</p><p>In the second sample, there are no debts.</p><p>In the third sample, you can annul all the debts.</p>
