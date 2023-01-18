## Description

<div><p>Polycarpus got hold of a family relationship tree. The tree describes family relationships of <span class="tex-span"><i>n</i></span> people, numbered 1 through <span class="tex-span"><i>n</i></span>. Each person in the tree has no more than one parent.</p><p>Let's call person <span class="tex-span"><i>a</i></span> a 1-ancestor of person <span class="tex-span"><i>b</i></span>, if <span class="tex-span"><i>a</i></span> is the parent of <span class="tex-span"><i>b</i></span>.</p><p>Let's call person <span class="tex-span"><i>a</i></span> a <span class="tex-span"><i>k</i></span>-ancestor <span class="tex-span">(<i>k</i> &gt; 1)</span> of person <span class="tex-span"><i>b</i></span>, if person <span class="tex-span"><i>b</i></span> has a 1-ancestor, and <span class="tex-span"><i>a</i></span> is a <span class="tex-span">(<i>k</i> - 1)</span>-ancestor of <span class="tex-span"><i>b</i></span>'s 1-ancestor. </p><p>Family relationships don't form cycles in the found tree. In other words, there is no person who is his own ancestor, directly or indirectly (that is, who is an <span class="tex-span"><i>x</i></span>-ancestor for himself, for some <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>x</i> &gt; 0</span>).</p><p><span class="tex-font-style-bf">Let's call two people <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> <span class="tex-span">(<i>x</i> ≠ <i>y</i>)</span> <span class="tex-span"><i>p</i></span>-th cousins <span class="tex-span">(<i>p</i> &gt; 0)</span>, if there is person <span class="tex-span"><i>z</i></span>, who is a <span class="tex-span"><i>p</i></span>-ancestor of <span class="tex-span"><i>x</i></span> and a <span class="tex-span"><i>p</i></span>-ancestor of <span class="tex-span"><i>y</i></span>.</span></p><p>Polycarpus wonders how many counsins and what kinds of them everybody has. He took a piece of paper and wrote <span class="tex-span"><i>m</i></span> pairs of integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>. Help him to calculate the number of <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>-th cousins that person <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> has, for each pair <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="input-specification"><p>The first input line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of people in the tree. The next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>r</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub>, ..., <i>r</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> is the number of person <span class="tex-span"><i>i</i></span>'s parent or <span class="tex-font-style-tt">0</span>, if person <span class="tex-span"><i>i</i></span> has no parent. It is guaranteed that family relationships don't form cycles.</p><p>The third line contains a single number <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of family relationship queries Polycarus has. Next <span class="tex-span"><i>m</i></span> lines contain pairs of space-separated integers. The <span class="tex-span"><i>i</i></span>-th line contains numbers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> space-separated integers — the answers to Polycarpus' queries. Print the answers to the queries in the order, in which the queries occur in the input.</p></div>

## Input

<p>The first input line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of people in the tree. The next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>r</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub>, ..., <i>r</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> is the number of person <span class="tex-span"><i>i</i></span>'s parent or <span class="tex-font-style-tt">0</span>, if person <span class="tex-span"><i>i</i></span> has no parent. It is guaranteed that family relationships don't form cycles.</p><p>The third line contains a single number <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of family relationship queries Polycarus has. Next <span class="tex-span"><i>m</i></span> lines contain pairs of space-separated integers. The <span class="tex-span"><i>i</i></span>-th line contains numbers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> space-separated integers — the answers to Polycarpus' queries. Print the answers to the queries in the order, in which the queries occur in the input.</p>





```input1
6
0 1 1 0 4 4
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
0 0 1 0 0 1 1 

```


