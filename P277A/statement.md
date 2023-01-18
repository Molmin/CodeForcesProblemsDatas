## Description

<div><p>The "BerCorp" company has got <span class="tex-span"><i>n</i></span> employees. These employees can use <span class="tex-span"><i>m</i></span> approved official languages for the formal correspondence. The languages are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>. For each employee we have the list of languages, which he knows. This list could be empty, i. e. an employee may know no official languages. But the employees are willing to learn any number of official languages, as long as the company pays their lessons. A study course in one language for one employee costs <span class="tex-span">1</span> berdollar.</p><p>Find the minimum sum of money the company needs to spend so as any employee could correspond to any other one (their correspondence can be indirect, i. e. other employees can help out translating).</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 100</span>) — the number of employees and the number of languages.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow — each employee's language list. At the beginning of the <span class="tex-span"><i>i</i></span>-th line is integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>) — the number of languages the <span class="tex-span"><i>i</i></span>-th employee knows. Next, the <span class="tex-span"><i>i</i></span>-th line contains <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> integers — <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ <i>m</i></span>) — the identifiers of languages the <span class="tex-span"><i>i</i></span>-th employee knows. It is guaranteed that all the identifiers in one list are distinct. Note that an employee may know zero languages.</p><p>The numbers in the lines are separated by single spaces.</p></div><div class="output-specification"><p>Print a single integer — the minimum amount of money to pay so that in the end every employee could write a letter to every other one (other employees can help out translating).</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 100</span>) — the number of employees and the number of languages.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow — each employee's language list. At the beginning of the <span class="tex-span"><i>i</i></span>-th line is integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>) — the number of languages the <span class="tex-span"><i>i</i></span>-th employee knows. Next, the <span class="tex-span"><i>i</i></span>-th line contains <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> integers — <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ <i>m</i></span>) — the identifiers of languages the <span class="tex-span"><i>i</i></span>-th employee knows. It is guaranteed that all the identifiers in one list are distinct. Note that an employee may know zero languages.</p><p>The numbers in the lines are separated by single spaces.</p>

## Output

<p>Print a single integer — the minimum amount of money to pay so that in the end every employee could write a letter to every other one (other employees can help out translating).</p>





```input1
5 5
1 2
2 2 3
2 3 4
2 4 5
1 5

```




```input2
8 7
0
3 1 2 3
1 1
2 5 4
2 6 7
1 3
2 7 4
1 1

```




```input3
2 2
1 2
0

```




```output1
0

```




```output2
2

```




```output3
1

```



## Note

<p>In the second sample the employee <span class="tex-span">1</span> can learn language <span class="tex-span">2</span>, and employee <span class="tex-span">8</span> can learn language <span class="tex-span">4</span>.</p><p>In the third sample employee <span class="tex-span">2</span> must learn language <span class="tex-span">2</span>.</p>
