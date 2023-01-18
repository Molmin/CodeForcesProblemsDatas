## Description

<div><p><span class="tex-span"><i>T</i></span> is a complete binary tree consisting of <span class="tex-span"><i>n</i></span> vertices. It means that exactly one vertex is a root, and each vertex is either a leaf (and doesn't have children) or an inner node (and has exactly two children). All leaves of a complete binary tree have the same depth (distance from the root). So <span class="tex-span"><i>n</i></span> is a number such that <span class="tex-span"><i>n</i> + 1</span> is a power of <span class="tex-span">2</span>.</p><p>In the picture you can see a complete binary tree with <span class="tex-span"><i>n</i> = 15</span>.</p><center> <img class="tex-graphics" src="file://cmHP13eh.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Vertices are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in a special recursive way: we recursively assign numbers to all vertices from the left subtree (if current vertex is not a leaf), then assign a number to the current vertex, and then recursively assign numbers to all vertices from the right subtree (if it exists). In the picture vertices are numbered exactly using this algorithm. It is clear that for each size of a complete binary tree exists exactly one way to give numbers to all vertices. This way of numbering is called <span class="tex-font-style-it">symmetric</span>.</p><p>You have to write a program that for given <span class="tex-span"><i>n</i></span> answers <span class="tex-span"><i>q</i></span> queries to the tree.</p><p>Each query consists of an integer number <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) and a string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>, where <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> is the number of vertex, and <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> represents the path starting from this vertex. String <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> doesn't contain any characters other than '<span class="tex-font-style-tt">L</span>', '<span class="tex-font-style-tt">R</span>' and '<span class="tex-font-style-tt">U</span>', which mean traverse to the left child, to the right child and to the parent, respectively. Characters from <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> have to be processed from left to right, considering that <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> is the vertex where the path starts. If it's impossible to process a character (for example, to go to the left child of a leaf), then you have to skip it. The answer is the number of vertex where the path represented by <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> ends.</p><p>For example, if <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> = 4</span> and <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> = </span>«<span class="tex-font-style-tt">UURL</span>», then the answer is <span class="tex-span">10</span>.</p></div><div class="input-specification"><p>The first line contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span"><i>q</i> ≥ 1</span>). <span class="tex-span"><i>n</i></span> is such that <span class="tex-span"><i>n</i> + 1</span> is a power of <span class="tex-span">2</span>.</p><p>The next <span class="tex-span">2<i>q</i></span> lines represent queries; each query consists of two consecutive lines. The first of these two lines contains <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), the second contains non-empty string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>. <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> doesn't contain any characters other than '<span class="tex-font-style-tt">L</span>', '<span class="tex-font-style-tt">R</span>' and '<span class="tex-font-style-tt">U</span>'.</p><p>It is guaranteed that the sum of lengths of <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (for each <span class="tex-span"><i>i</i></span> such that <span class="tex-span">1 ≤ <i>i</i> ≤ <i>q</i></span>) doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>q</i></span> numbers, <span class="tex-span"><i>i</i></span>-th number must be the answer to the <span class="tex-span"><i>i</i></span>-th query.</p></div>

## Input

<p>The first line contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span"><i>q</i> ≥ 1</span>). <span class="tex-span"><i>n</i></span> is such that <span class="tex-span"><i>n</i> + 1</span> is a power of <span class="tex-span">2</span>.</p><p>The next <span class="tex-span">2<i>q</i></span> lines represent queries; each query consists of two consecutive lines. The first of these two lines contains <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), the second contains non-empty string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>. <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> doesn't contain any characters other than '<span class="tex-font-style-tt">L</span>', '<span class="tex-font-style-tt">R</span>' and '<span class="tex-font-style-tt">U</span>'.</p><p>It is guaranteed that the sum of lengths of <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (for each <span class="tex-span"><i>i</i></span> such that <span class="tex-span">1 ≤ <i>i</i> ≤ <i>q</i></span>) doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p>

## Output

<p>Print <span class="tex-span"><i>q</i></span> numbers, <span class="tex-span"><i>i</i></span>-th number must be the answer to the <span class="tex-span"><i>i</i></span>-th query.</p>





```input1
15 2
4
UURL
8
LRLLLLLLLL

```




```output1
10
5

```


