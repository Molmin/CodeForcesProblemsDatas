## Description

<div><p>You need to find a binary tree of size <span class="tex-span"><i>n</i></span> that satisfies a given set of <span class="tex-span"><i>c</i></span> constraints. Suppose that the nodes of the unknown binary tree are labeled using a <span class="tex-font-style-it">pre-order</span> traversal starting with <span class="tex-span">1</span>. For the <span class="tex-span"><i>i</i></span>-th constraint you are given two labels, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and a direction, left or right. In case of left direction, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is an element of the subtree rooted at <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>'s left child. Similarly in the case of right direction <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is an element of the subtree rooted at <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>'s right child.</p></div><div class="input-specification"><p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>c</i></span>. The next <span class="tex-span"><i>c</i></span> lines contain 2 integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) and either "<span class="tex-font-style-tt">LEFT</span>" or "<span class="tex-font-style-tt">RIGHT</span>" denoting whether <span class="tex-span"><i>b</i></span> is in the subtree rooted at <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>'s left child or in the subtree rooted at <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>'s right child.</p><p><span class="tex-font-style-it">The problem consists of multiple subproblems. The subproblems have different constraints on the input. You will get some score for the correct submission of the subproblem. The description of the subproblems follows.</span></p><ul> <li> In subproblem D1 (<span class="tex-span">9</span> points), the constraints <span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>c</i> ≤ 50</span> will hold. </li><li> In subproblem D2 (<span class="tex-span">8</span> points), the constraints <span class="tex-span">1 ≤ <i>n</i> ≤ 1000000</span>, <span class="tex-span">1 ≤ <i>c</i> ≤ 100000</span> will hold. </li></ul></div><div class="output-specification"><p>Output will be on a single line.</p><p>Any binary tree that satisfies the constraints will be accepted. The tree's nodes should be printed out as <span class="tex-span"><i>n</i></span> space separated labels representing an <span class="tex-font-style-it">in-order</span> traversal, using the <span class="tex-font-style-it">pre-order</span> numbers as labels of vertices.</p><p>If there are no trees that satisfy the constraints, print "<span class="tex-font-style-tt">IMPOSSIBLE</span>" (without quotes).</p></div>

## Input

<p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>c</i></span>. The next <span class="tex-span"><i>c</i></span> lines contain 2 integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) and either "<span class="tex-font-style-tt">LEFT</span>" or "<span class="tex-font-style-tt">RIGHT</span>" denoting whether <span class="tex-span"><i>b</i></span> is in the subtree rooted at <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>'s left child or in the subtree rooted at <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>'s right child.</p><p><span class="tex-font-style-it">The problem consists of multiple subproblems. The subproblems have different constraints on the input. You will get some score for the correct submission of the subproblem. The description of the subproblems follows.</span></p><ul> <li> In subproblem D1 (<span class="tex-span">9</span> points), the constraints <span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>c</i> ≤ 50</span> will hold. </li><li> In subproblem D2 (<span class="tex-span">8</span> points), the constraints <span class="tex-span">1 ≤ <i>n</i> ≤ 1000000</span>, <span class="tex-span">1 ≤ <i>c</i> ≤ 100000</span> will hold. </li></ul>

## Output

<p>Output will be on a single line.</p><p>Any binary tree that satisfies the constraints will be accepted. The tree's nodes should be printed out as <span class="tex-span"><i>n</i></span> space separated labels representing an <span class="tex-font-style-it">in-order</span> traversal, using the <span class="tex-font-style-it">pre-order</span> numbers as labels of vertices.</p><p>If there are no trees that satisfy the constraints, print "<span class="tex-font-style-tt">IMPOSSIBLE</span>" (without quotes).</p>





```input1
3 2
1 2 LEFT
1 3 RIGHT

```




```input2
3 2
1 2 RIGHT
1 3 LEFT

```




```output1
2 1 3

```




```output2
IMPOSSIBLE

```



## Note

<p>Consider the first sample test. We need to find a tree with 3 nodes that satisfies the following two constraints. The node labeled 2 with pre-order traversal should be in the left subtree of the node labeled 1 with pre-order traversal; the node labeled 3 with pre-order traversal should be in the right subtree of the node labeled 1. There is only one tree with three nodes that satisfies these constraints and its in-order traversal is <span class="tex-span">(2, 1, 3)</span>.</p><p><span class="tex-font-style-it">Pre-order</span> is the "root – left subtree – right subtree" order. <span class="tex-font-style-it">In-order</span> is the "left subtree – root – right subtree" order.</p><p>For other information regarding <span class="tex-font-style-it">in-order</span> and <span class="tex-font-style-it">pre-order</span>, see <a href="http://en.wikipedia.org/wiki/Tree_traversal">http://en.wikipedia.org/wiki/Tree_traversal</a>.</p>
