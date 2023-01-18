## Description

<div><p>Oscolcovo city has a campus consisting of <span class="tex-span"><i>n</i></span> student dormitories, <span class="tex-span"><i>n</i></span> universities and <span class="tex-span"><i>n</i></span> military offices. Initially, the <span class="tex-span"><i>i</i></span>-th dormitory belongs to the <span class="tex-span"><i>i</i></span>-th university and is assigned to the <span class="tex-span"><i>i</i></span>-th military office.</p><p>Life goes on and the campus is continuously going through some changes. The changes can be of four types:</p><ol> <li> University <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> merges with university <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span>. After that all the dormitories that belonged to university <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> are assigned to to university <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span>, and university <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> disappears. </li><li> Military office <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub></span> merges with military office <span class="tex-span"><i>d</i><sub class="lower-index"><i>j</i></sub></span>. After that all the dormitories that were assigned to military office <span class="tex-span"><i>d</i><sub class="lower-index"><i>j</i></sub></span>, are assigned to military office <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub></span>, and military office <span class="tex-span"><i>d</i><sub class="lower-index"><i>j</i></sub></span> disappears. </li><li> Students of university <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span> move in dormitories. Lets <span class="tex-span"><i>k</i><sub class="lower-index"><i>x</i><sub class="lower-index"><i>j</i></sub></sub></span> is the number of dormitories that belong to this university at the time when the students move in. Then the number of students in each dormitory of university <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span> increases by <span class="tex-span"><i>k</i><sub class="lower-index"><i>x</i><sub class="lower-index"><i>j</i></sub></sub></span> (note that the more dormitories belong to the university, the more students move in each dormitory of the university). </li><li> Military office number <span class="tex-span"><i>y</i><sub class="lower-index"><i>j</i></sub></span> conducts raids on all the dormitories assigned to it and takes all students from there. </li></ol><p>Thus, at each moment of time each dormitory is assigned to exactly one university and one military office. Initially, all the dormitory are empty.</p><p>Your task is to process the changes that take place in the campus and answer the queries, how many people currently live in dormitory <span class="tex-span"><i>q</i><sub class="lower-index"><i>j</i></sub></span>.</p></div><div class="input-specification"><p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 5·10<sup class="upper-index">5</sup>)</span> — the number of dormitories and the number of queries, respectively.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain the queries, each of them is given in one of the following formats: </p><ul> <li> «<span class="tex-font-style-tt">U</span> <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span>» — merging universities; </li><li> «<span class="tex-font-style-tt">M</span> <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub></span> <span class="tex-span"><i>d</i><sub class="lower-index"><i>j</i></sub></span>» — merging military offices; </li><li> «<span class="tex-font-style-tt">A</span> <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span>» — students of university <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span> moving in the dormitories; </li><li> «<span class="tex-font-style-tt">Z</span> <span class="tex-span"><i>y</i><sub class="lower-index"><i>j</i></sub></span>» — a raid in military office <span class="tex-span"><i>y</i><sub class="lower-index"><i>j</i></sub></span>; </li><li> «<span class="tex-font-style-tt">Q</span> <span class="tex-span"><i>q</i><sub class="lower-index"><i>j</i></sub></span>» — a query asking the number of people in dormitory <span class="tex-span"><i>q</i><sub class="lower-index"><i>j</i></sub></span>. </li></ul> All the numbers in the queries are positive integers and do not exceed <span class="tex-span"><i>n</i></span>. It is guaranteed that at the moment of the query the universities and military offices, that are present in the query, exist.</div><div class="output-specification"><p>In the <span class="tex-span"><i>i</i></span>-th line print the answer to the <span class="tex-span"><i>i</i></span>-th query asking the number of people in the dormitory.</p></div>

## Input

<p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 5·10<sup class="upper-index">5</sup>)</span> — the number of dormitories and the number of queries, respectively.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain the queries, each of them is given in one of the following formats: </p><ul> <li> «<span class="tex-font-style-tt">U</span> <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span>» — merging universities; </li><li> «<span class="tex-font-style-tt">M</span> <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub></span> <span class="tex-span"><i>d</i><sub class="lower-index"><i>j</i></sub></span>» — merging military offices; </li><li> «<span class="tex-font-style-tt">A</span> <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span>» — students of university <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span> moving in the dormitories; </li><li> «<span class="tex-font-style-tt">Z</span> <span class="tex-span"><i>y</i><sub class="lower-index"><i>j</i></sub></span>» — a raid in military office <span class="tex-span"><i>y</i><sub class="lower-index"><i>j</i></sub></span>; </li><li> «<span class="tex-font-style-tt">Q</span> <span class="tex-span"><i>q</i><sub class="lower-index"><i>j</i></sub></span>» — a query asking the number of people in dormitory <span class="tex-span"><i>q</i><sub class="lower-index"><i>j</i></sub></span>. </li></ul> All the numbers in the queries are positive integers and do not exceed <span class="tex-span"><i>n</i></span>. It is guaranteed that at the moment of the query the universities and military offices, that are present in the query, exist.

## Output

<p>In the <span class="tex-span"><i>i</i></span>-th line print the answer to the <span class="tex-span"><i>i</i></span>-th query asking the number of people in the dormitory.</p>





```input1
2 7
A 1
Q 1
U 1 2
A 1
Z 1
Q 1
Q 2

```




```input2
5 12
U 1 2
M 4 5
A 1
Q 1
A 3
A 4
Q 3
Q 4
Z 4
Q 4
A 5
Q 5

```




```output1
1
0
2

```




```output2
2
1
1
0
1

```



## Note

<p>Consider the first sample test: </p><ul> <li> In the first query university 1 owns only dormitory 1, so after the query dormitory 1 will have 1 student. </li><li> After the third query university 1 owns dormitories 1 and 2. </li><li> The fourth query increases by 2 the number of students living in dormitories 1 and 2 that belong to university number 1. After that 3 students live in the first dormitory and 2 students live in the second dormitory. </li><li> At the fifth query the number of students living in dormitory 1, assigned to the military office 1, becomes zero. </li></ul>
