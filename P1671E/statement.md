## Description

<div><p>You are given a rooted tree of $2^n - 1$ vertices. Every vertex of this tree has either $0$ children, or $2$ children. All leaves of this tree have the same distance from the root, and for every non-leaf vertex, one of its children is the left one, and the other child is the right one. Formally, you are given a <span class="tex-font-style-it">perfect binary tree</span>.</p><p>The vertices of the tree are numbered in the following order:</p><ul> <li> the root has index $1$; </li><li> if a vertex has index $x$, then its left child has index $2x$, and its right child has index $2x+1$. </li></ul><p>Every vertex of the tree has a letter written on it, either <span class="tex-font-style-tt">A</span> or <span class="tex-font-style-tt">B</span>. Let's define the character on the vertex $x$ as $s_x$.</p><p>Let the <span class="tex-font-style-it">preorder string</span> of some vertex $x$ be defined in the following way:</p><ul> <li> if the vertex $x$ is a leaf, then the <span class="tex-font-style-it">preorder string</span> of $x$ be consisting of only one character $s_x$; </li><li> otherwise, the <span class="tex-font-style-it">preorder string</span> of $x$ is $s_x + f(l_x) + f(r_x)$, where $+$ operator defines concatenation of strings, $f(l_x)$ is the <span class="tex-font-style-it">preorder string</span> of the left child of $x$, and $f(r_x)$ is the <span class="tex-font-style-it">preorder string</span> of the right child of $x$. </li></ul><p>The <span class="tex-font-style-it">preorder string</span> of the tree is the <span class="tex-font-style-it">preorder string</span> of its root.</p><p><span class="tex-font-style-it">Now, for the problem itself...</span></p><p>You have to calculate the number of different strings that can be obtained as the <span class="tex-font-style-it">preorder string</span> of the given tree, if you are allowed to perform the following operation any number of times before constructing the <span class="tex-font-style-it">preorder string</span> of the tree:</p><ul> <li> choose any non-leaf vertex $x$, and swap its children (so, the left child becomes the right one, and vice versa). </li></ul></div><div class="input-specification"><p>The first line contains one integer $n$ ($2 \le n \le 18$).</p><p>The second line contains a sequence of $2^n-1$ characters $s_1, s_2, \dots, s_{2^n-1}$. Each character is either <span class="tex-font-style-tt">A</span> or <span class="tex-font-style-tt">B</span>. The characters are <span class="tex-font-style-bf">not separated</span> by spaces or anything else.</p></div><div class="output-specification"><p>Print one integer — the number of different strings that can be obtained as the <span class="tex-font-style-it">preorder string</span> of the given tree, if you can apply any number of operations described in the statement. Since it can be very large, print it modulo $998244353$.</p></div>

## Input

<p>The first line contains one integer $n$ ($2 \le n \le 18$).</p><p>The second line contains a sequence of $2^n-1$ characters $s_1, s_2, \dots, s_{2^n-1}$. Each character is either <span class="tex-font-style-tt">A</span> or <span class="tex-font-style-tt">B</span>. The characters are <span class="tex-font-style-bf">not separated</span> by spaces or anything else.</p>

## Output

<p>Print one integer — the number of different strings that can be obtained as the <span class="tex-font-style-it">preorder string</span> of the given tree, if you can apply any number of operations described in the statement. Since it can be very large, print it modulo $998244353$.</p>





```input1
4
BAAAAAAAABBABAB
```




```input2
2
BAA
```




```input3
2
ABA
```




```input4
2
AAB
```




```input5
2
AAA
```




```output1
16
```




```output2
1
```




```output3
2
```




```output4
2
```




```output5
1
```


