## Description

<div><p>Jack decides to invite Emma out for a dinner. Jack is a modest student, he doesn't want to go to an expensive restaurant. Emma is a girl with high taste, she prefers elite places.</p><p>Munhattan consists of <span class="tex-span"><i>n</i></span> streets and <span class="tex-span"><i>m</i></span> avenues. There is exactly one restaurant on the intersection of each street and avenue. The streets are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> and the avenues are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>. The cost of dinner in the restaurant at the intersection of the <span class="tex-span"><i>i</i></span>-th street and the <span class="tex-span"><i>j</i></span>-th avenue is <span class="tex-span"><i>c</i><sub class="lower-index"><i>ij</i></sub></span>.</p><p>Jack and Emma decide to choose the restaurant in the following way. Firstly Emma chooses the street to dinner and then Jack chooses the avenue. Emma and Jack makes their choice optimally: Emma wants to maximize the cost of the dinner, Jack wants to minimize it. Emma takes into account that Jack wants to minimize the cost of the dinner. Find the cost of the dinner for the couple in love.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>) — the number of streets and avenues in Munhattan.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>ij</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the cost of the dinner in the restaurant on the intersection of the <span class="tex-span"><i>i</i></span>-th street and the <span class="tex-span"><i>j</i></span>-th avenue.</p></div><div class="output-specification"><p>Print the only integer <span class="tex-span"><i>a</i></span> — the cost of the dinner for Jack and Emma.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>) — the number of streets and avenues in Munhattan.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>ij</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the cost of the dinner in the restaurant on the intersection of the <span class="tex-span"><i>i</i></span>-th street and the <span class="tex-span"><i>j</i></span>-th avenue.</p>

## Output

<p>Print the only integer <span class="tex-span"><i>a</i></span> — the cost of the dinner for Jack and Emma.</p>





```input1
3 4
4 1 3 5
2 2 2 2
5 4 5 1

```




```input2
3 3
1 2 3
2 3 1
3 1 2

```




```output1
2

```




```output2
1

```



## Note

<p>In the first example if Emma chooses the first or the third streets Jack can choose an avenue with the cost of the dinner <span class="tex-span">1</span>. So she chooses the second street and Jack chooses any avenue. The cost of the dinner is <span class="tex-span">2</span>.</p><p>In the second example regardless of Emma's choice Jack can choose a restaurant with the cost of the dinner <span class="tex-span">1</span>.</p>
