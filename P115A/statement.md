## Description

<div><p>A company has <span class="tex-span"><i>n</i></span> employees numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Each employee either has no immediate manager or exactly one immediate manager, who is another employee with a different number. An employee <span class="tex-span"><i>A</i></span> is said to be the <span class="tex-font-style-underline">superior</span> of another employee <span class="tex-span"><i>B</i></span> if at least one of the following is true:</p><ul> <li> Employee <span class="tex-span"><i>A</i></span> is the immediate manager of employee <span class="tex-span"><i>B</i></span> </li><li> Employee <span class="tex-span"><i>B</i></span> has an immediate manager employee <span class="tex-span"><i>C</i></span> such that employee <span class="tex-span"><i>A</i></span> is the superior of employee <span class="tex-span"><i>C</i></span>. </li></ul><p>The company will not have a managerial cycle. That is, there will not exist an employee who is the superior of his/her own immediate manager.</p><p>Today the company is going to arrange a party. This involves dividing all <span class="tex-span"><i>n</i></span> employees into several groups: every employee must belong to exactly one group. Furthermore, within any single group, there must not be two employees <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> such that <span class="tex-span"><i>A</i></span> is the superior of <span class="tex-span"><i>B</i></span>.</p><p>What is the minimum number of groups that must be formed?</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>) — the number of employees.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span> or <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> = </span>-1). Every <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> denotes the immediate manager for the <span class="tex-span"><i>i</i></span>-th employee. If <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is -1, that means that the <span class="tex-span"><i>i</i></span>-th employee does not have an immediate manager. </p><p>It is guaranteed, that no employee will be the immediate manager of him/herself (<span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> ≠ <i>i</i></span>). Also, there will be no managerial cycles.</p></div><div class="output-specification"><p>Print a single integer denoting the minimum number of groups that will be formed in the party.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>) — the number of employees.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span> or <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> = </span>-1). Every <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> denotes the immediate manager for the <span class="tex-span"><i>i</i></span>-th employee. If <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is -1, that means that the <span class="tex-span"><i>i</i></span>-th employee does not have an immediate manager. </p><p>It is guaranteed, that no employee will be the immediate manager of him/herself (<span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> ≠ <i>i</i></span>). Also, there will be no managerial cycles.</p>

## Output

<p>Print a single integer denoting the minimum number of groups that will be formed in the party.</p>





```input1
5
-1
1
2
1
-1

```




```output1
3

```



## Note

<p>For the first example, three groups are sufficient, for example: </p><ul> <li> Employee 1 </li><li> Employees 2 and 4 </li><li> Employees 3 and 5 </li></ul>
