## Description

<div><p>Masha and Grisha like studying sets of positive integers.</p><p>One day Grisha has written a set <span class="tex-span"><i>A</i></span> containing <span class="tex-span"><i>n</i></span> different integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> on a blackboard. Now he asks Masha to create a set <span class="tex-span"><i>B</i></span> containing <span class="tex-span"><i>n</i></span> different integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> such that all <span class="tex-span"><i>n</i><sup class="upper-index">2</sup></span> integers that can be obtained by summing up <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> for all possible pairs of <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> are different.</p><p>Both Masha and Grisha don't like big numbers, so all numbers in <span class="tex-span"><i>A</i></span> are from <span class="tex-span">1</span> to <span class="tex-span">10<sup class="upper-index">6</sup></span>, and all numbers in <span class="tex-span"><i>B</i></span> must also be in the same range.</p><p>Help Masha to create the set <span class="tex-span"><i>B</i></span> that satisfies Grisha's requirement.</p></div><div class="input-specification"><p>Input data contains multiple test cases. The first line contains an integer <span class="tex-span"><i>t</i></span>&nbsp;— the number of test cases (<span class="tex-span">1 ≤ <i>t</i> ≤ 100</span>).</p><p>Each test case is described in the following way: the first line of the description contains one integer <span class="tex-span"><i>n</i></span>&nbsp;— the number of elements in <span class="tex-span"><i>A</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— the elements of <span class="tex-span"><i>A</i></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>). </p></div><div class="output-specification"><p>For each test first print the answer: </p><ul> <li> <span class="tex-font-style-tt">NO</span>, if Masha's task is impossible to solve, there is no way to create the required set <span class="tex-span"><i>B</i></span>. </li><li> <span class="tex-font-style-tt">YES</span>, if there is the way to create the required set. In this case the second line must contain <span class="tex-span"><i>n</i></span> different positive integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span>&nbsp;— elements of <span class="tex-span"><i>B</i></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">6</sup></span>). If there are several possible sets, output any of them. </li></ul></div>

## Input

<p>Input data contains multiple test cases. The first line contains an integer <span class="tex-span"><i>t</i></span>&nbsp;— the number of test cases (<span class="tex-span">1 ≤ <i>t</i> ≤ 100</span>).</p><p>Each test case is described in the following way: the first line of the description contains one integer <span class="tex-span"><i>n</i></span>&nbsp;— the number of elements in <span class="tex-span"><i>A</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— the elements of <span class="tex-span"><i>A</i></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>). </p>

## Output

<p>For each test first print the answer: </p><ul> <li> <span class="tex-font-style-tt">NO</span>, if Masha's task is impossible to solve, there is no way to create the required set <span class="tex-span"><i>B</i></span>. </li><li> <span class="tex-font-style-tt">YES</span>, if there is the way to create the required set. In this case the second line must contain <span class="tex-span"><i>n</i></span> different positive integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span>&nbsp;— elements of <span class="tex-span"><i>B</i></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">6</sup></span>). If there are several possible sets, output any of them. </li></ul>





```input1
3
3
1 10 100
1
1
2
2 4

```




```output1
YES
1 2 3 
YES
1 
YES
1 2 

```


