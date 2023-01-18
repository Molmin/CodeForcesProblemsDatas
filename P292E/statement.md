## Description

<div><p>We often have to copy large volumes of information. Such operation can take up many computer resources. Therefore, in this problem you are advised to come up with a way to copy some part of a number array into another one, quickly.</p><p>More formally, you've got two arrays of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> of length <span class="tex-span"><i>n</i></span>. Also, you've got <span class="tex-span"><i>m</i></span> queries of two types:</p><ol> <li> Copy the subsegment of array <span class="tex-span"><i>a</i></span> of length <span class="tex-span"><i>k</i></span>, starting from position <span class="tex-span"><i>x</i></span>, into array <span class="tex-span"><i>b</i></span>, starting from position <span class="tex-span"><i>y</i></span>, that is, execute <span class="tex-span"><i>b</i><sub class="lower-index"><i>y</i> + <i>q</i></sub> = <i>a</i><sub class="lower-index"><i>x</i> + <i>q</i></sub></span> for all integer <span class="tex-span"><i>q</i></span> <span class="tex-span">(0 ≤ <i>q</i> &lt; <i>k</i>)</span>. The given operation is correct — both subsegments do not touch unexistent elements. </li><li> Determine the value in position <span class="tex-span"><i>x</i></span> of array <span class="tex-span"><i>b</i></span>, that is, find value <span class="tex-span"><i>b</i><sub class="lower-index"><i>x</i></sub></span>. </li></ol><p>For each query of the second type print the result — the value of the corresponding element of array <span class="tex-span"><i>b</i></span>.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of elements in the arrays and the number of queries, correspondingly. The second line contains an array of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup>)</span>. The third line contains an array of integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(|<i>b</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup>)</span>.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain the descriptions of the queries. The <span class="tex-span"><i>i</i></span>-th line first contains integer <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> — the type of the <span class="tex-span"><i>i</i></span>-th query <span class="tex-span">(1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2)</span>. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 1</span>, then the <span class="tex-span"><i>i</i></span>-th query means the copying operation. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 2</span>, then the <span class="tex-span"><i>i</i></span>-th query means taking the value in array <span class="tex-span"><i>b</i></span>. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 1</span>, then the query type is followed by three integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>, <i>k</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>, <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the parameters of the copying query. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 2</span>, then the query type is followed by integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the position in array <span class="tex-span"><i>b</i></span>.</p><p>All numbers in the lines are separated with single spaces. It is guaranteed that all the queries are correct, that is, the copying borders fit into the borders of arrays <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>.</p></div><div class="output-specification"><p>For each second type query print the result on a single line.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of elements in the arrays and the number of queries, correspondingly. The second line contains an array of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup>)</span>. The third line contains an array of integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(|<i>b</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup>)</span>.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain the descriptions of the queries. The <span class="tex-span"><i>i</i></span>-th line first contains integer <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> — the type of the <span class="tex-span"><i>i</i></span>-th query <span class="tex-span">(1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2)</span>. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 1</span>, then the <span class="tex-span"><i>i</i></span>-th query means the copying operation. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 2</span>, then the <span class="tex-span"><i>i</i></span>-th query means taking the value in array <span class="tex-span"><i>b</i></span>. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 1</span>, then the query type is followed by three integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>, <i>k</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>, <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the parameters of the copying query. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 2</span>, then the query type is followed by integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the position in array <span class="tex-span"><i>b</i></span>.</p><p>All numbers in the lines are separated with single spaces. It is guaranteed that all the queries are correct, that is, the copying borders fit into the borders of arrays <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>.</p>

## Output

<p>For each second type query print the result on a single line.</p>





```input1
5 10
1 2 0 -1 3
3 1 5 -2 0
2 5
1 3 3 3
2 5
2 4
2 1
1 2 1 4
2 1
2 4
1 4 2 1
2 2

```




```output1
0
3
-1
3
2
3
-1

```


