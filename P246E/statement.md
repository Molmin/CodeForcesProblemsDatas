## Description

<div><p>Polycarpus got hold of a family tree. The found tree describes the family relations of <span class="tex-span"><i>n</i></span> people, numbered from 1 to <span class="tex-span"><i>n</i></span>. Every person in this tree has at most one direct ancestor. Also, each person in the tree has a name, the names are not necessarily unique.</p><p>We call the man with a number <span class="tex-span"><i>a</i></span> a 1-ancestor of the man with a number <span class="tex-span"><i>b</i></span>, if the man with a number <span class="tex-span"><i>a</i></span> is a direct ancestor of the man with a number <span class="tex-span"><i>b</i></span>.</p><p>We call the man with a number <span class="tex-span"><i>a</i></span> a <span class="tex-span"><i>k</i></span>-ancestor <span class="tex-span">(<i>k</i> &gt; 1)</span> of the man with a number <span class="tex-span"><i>b</i></span>, if the man with a number <span class="tex-span"><i>b</i></span> has a 1-ancestor, and the man with a number <span class="tex-span"><i>a</i></span> is a <span class="tex-span">(<i>k</i> - 1)</span>-ancestor of the 1-ancestor of the man with a number <span class="tex-span"><i>b</i></span>.</p><p>In the tree the family ties do not form cycles. In other words there isn't a person who is his own direct or indirect ancestor (that is, who is an <span class="tex-span"><i>x</i></span>-ancestor of himself, for some <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>x</i> &gt; 0</span>).</p><p>We call a man with a number <span class="tex-span"><i>a</i></span> the <span class="tex-span"><i>k</i></span>-son of the man with a number <span class="tex-span"><i>b</i></span>, if the man with a number <span class="tex-span"><i>b</i></span> is a <span class="tex-span"><i>k</i></span>-ancestor of the man with a number <span class="tex-span"><i>a</i></span>.</p><p>Polycarpus is very much interested in how many sons and which sons each person has. He took a piece of paper and wrote <span class="tex-span"><i>m</i></span> pairs of numbers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>. Help him to learn for each pair <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> the number of distinct names among all names of the <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>-sons of the man with number <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of people in the tree. Next <span class="tex-span"><i>n</i></span> lines contain the description of people in the tree. The <span class="tex-span"><i>i</i></span>-th line contains space-separated string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and integer <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>, where <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> is the name of the man with a number <span class="tex-span"><i>i</i></span>, and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> is either the number of the direct ancestor of the man with a number <span class="tex-span"><i>i</i></span> or <span class="tex-font-style-tt">0</span>, if the man with a number <span class="tex-span"><i>i</i></span> has no direct ancestor. </p><p>The next line contains a single integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of Polycarpus's records. Next <span class="tex-span"><i>m</i></span> lines contain space-separated pairs of integers. The <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>.</p><p>It is guaranteed that the family relationships do not form cycles. The names of all people are non-empty strings, consisting of no more than 20 lowercase English letters.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> whitespace-separated integers — the answers to Polycarpus's records. Print the answers to the records in the order, in which the records occur in the input.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of people in the tree. Next <span class="tex-span"><i>n</i></span> lines contain the description of people in the tree. The <span class="tex-span"><i>i</i></span>-th line contains space-separated string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and integer <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>, where <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> is the name of the man with a number <span class="tex-span"><i>i</i></span>, and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> is either the number of the direct ancestor of the man with a number <span class="tex-span"><i>i</i></span> or <span class="tex-font-style-tt">0</span>, if the man with a number <span class="tex-span"><i>i</i></span> has no direct ancestor. </p><p>The next line contains a single integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of Polycarpus's records. Next <span class="tex-span"><i>m</i></span> lines contain space-separated pairs of integers. The <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>.</p><p>It is guaranteed that the family relationships do not form cycles. The names of all people are non-empty strings, consisting of no more than 20 lowercase English letters.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> whitespace-separated integers — the answers to Polycarpus's records. Print the answers to the records in the order, in which the records occur in the input.</p>





```input1
6
pasha 0
gerald 1
gerald 1
valera 2
igor 3
olesya 1
5
1 1
1 2
1 3
3 1
6 1

```




```input2
6
valera 0
valera 1
valera 1
gerald 0
valera 4
kolya 4
7
1 1
1 2
2 1
2 2
4 1
5 1
6 1

```




```output1
2
2
0
1
0

```




```output2
1
0
0
0
2
0
0

```


