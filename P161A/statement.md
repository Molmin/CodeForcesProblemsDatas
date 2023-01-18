## Description

<div><p>The Two-dimensional kingdom is going through hard times... This morning the Three-Dimensional kingdom declared war on the Two-dimensional one. This (possibly armed) conflict will determine the ultimate owner of the straight line.</p><p>The Two-dimensional kingdom has a regular army of <span class="tex-span"><i>n</i></span> people. Each soldier registered himself and indicated the desired size of the bulletproof vest: the <span class="tex-span"><i>i</i></span>-th soldier indicated size <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. The soldiers are known to be unpretentious, so the command staff assumes that the soldiers are comfortable in any vests with sizes from <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> - <i>x</i></span> to <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> + <i>y</i></span>, inclusive (numbers <span class="tex-span"><i>x</i>, <i>y</i> ≥ 0</span> are specified). </p><p>The Two-dimensional kingdom has <span class="tex-span"><i>m</i></span> vests at its disposal, the <span class="tex-span"><i>j</i></span>-th vest's size equals <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span>. Help mobilize the Two-dimensional kingdom's army: equip with vests as many soldiers as possible. Each vest can be used only once. The <span class="tex-span"><i>i</i></span>-th soldier can put on the <span class="tex-span"><i>j</i></span>-th vest, if <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> - <i>x</i> ≤ <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> + <i>y</i></span>.</p></div><div class="input-specification"><p>The first input line contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of soldiers, the number of vests and two numbers that specify the soldiers' unpretentiousness, correspondingly.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) in non-decreasing order, separated by single spaces — the desired sizes of vests. </p><p>The third line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) in non-decreasing order, separated by single spaces — the sizes of the available vests.</p></div><div class="output-specification"><p>In the first line print a single integer <span class="tex-span"><i>k</i></span> — the maximum number of soldiers equipped with bulletproof vests. </p><p>In the next <span class="tex-span"><i>k</i></span> lines print <span class="tex-span"><i>k</i></span> pairs, one pair per line, as "<span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>" (without the quotes). Pair (<span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>) means that soldier number <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> must wear vest number <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. Soldiers and vests are numbered starting from one in the order in which they are specified in the input. All numbers of soldiers in the pairs should be pairwise different, all numbers of vests in the pairs also should be pairwise different. You can print the pairs in any order.</p><p>If there are multiple optimal answers, you are allowed to print any of them.</p></div>

## Input

<p>The first input line contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of soldiers, the number of vests and two numbers that specify the soldiers' unpretentiousness, correspondingly.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) in non-decreasing order, separated by single spaces — the desired sizes of vests. </p><p>The third line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) in non-decreasing order, separated by single spaces — the sizes of the available vests.</p>

## Output

<p>In the first line print a single integer <span class="tex-span"><i>k</i></span> — the maximum number of soldiers equipped with bulletproof vests. </p><p>In the next <span class="tex-span"><i>k</i></span> lines print <span class="tex-span"><i>k</i></span> pairs, one pair per line, as "<span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>" (without the quotes). Pair (<span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>) means that soldier number <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> must wear vest number <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. Soldiers and vests are numbered starting from one in the order in which they are specified in the input. All numbers of soldiers in the pairs should be pairwise different, all numbers of vests in the pairs also should be pairwise different. You can print the pairs in any order.</p><p>If there are multiple optimal answers, you are allowed to print any of them.</p>





```input1
5 3 0 0
1 2 3 3 4
1 3 5

```




```input2
3 3 2 2
1 5 9
3 5 7

```




```output1
2
1 1
3 2

```




```output2
3
1 1
2 2
3 3

```



## Note

<p>In the first sample you need the vests' sizes to match perfectly: the first soldier gets the first vest (size 1), the third soldier gets the second vest (size 3). This sample allows another answer, which gives the second vest to the fourth soldier instead of the third one.</p><p>In the second sample the vest size can differ from the desired size by at most 2 sizes, so all soldiers can be equipped.</p>
