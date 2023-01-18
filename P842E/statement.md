## Description

<div><p>Nikita plays a new computer game. There are <span class="tex-span"><i>m</i></span> levels in this game. In the beginning of each level a new class appears in the game; this class is a child-class of the class <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> is called parent-class for this new class). Thus, the classes form a tree. Initially there is only one class with index <span class="tex-span">1</span>.</p><p>Changing the class to its neighbour (child-class or parent-class) in the tree costs <span class="tex-span">1</span> coin. You can not change the class back. The cost of changing the class <span class="tex-span"><i>a</i></span> to the class <span class="tex-span"><i>b</i></span> is equal to the total cost of class changes on the path from <span class="tex-span"><i>a</i></span> to <span class="tex-span"><i>b</i></span> in the class tree.</p><p>Suppose that at <span class="tex-span"><i>i</i></span>&nbsp;-th level the maximum cost of changing one class to another is <span class="tex-span"><i>x</i></span>. For each level output the number of classes such that for each of these classes there exists some other class <span class="tex-span"><i>y</i></span>, and the distance from this class to <span class="tex-span"><i>y</i></span> is exactly <span class="tex-span"><i>x</i></span>.</p></div><div class="input-specification"><p>First line contains one integer number <span class="tex-span"><i>m</i></span>&nbsp;— number of queries (<span class="tex-span">1 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>).</p><p>Next <span class="tex-span"><i>m</i></span> lines contain description of queries. <span class="tex-span"><i>i</i></span>&nbsp;-th line (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>m</i></span>) describes the <span class="tex-span"><i>i</i></span>&nbsp;-th level and contains an integer <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— the index of the parent-class of class with index <span class="tex-span"><i>i</i> + 1</span> (<span class="tex-span">1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>i</i></span>). </p></div><div class="output-specification"><p>Suppose that at <span class="tex-span"><i>i</i></span>&nbsp;-th level the maximum cost of changing one class to another is <span class="tex-span"><i>x</i></span>. For each level output the number of classes such that for each of these classes there exists some other class <span class="tex-span"><i>y</i></span>, and the distance from this class to <span class="tex-span"><i>y</i></span> is exactly <span class="tex-span"><i>x</i></span>.</p></div>

## Input

<p>First line contains one integer number <span class="tex-span"><i>m</i></span>&nbsp;— number of queries (<span class="tex-span">1 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>).</p><p>Next <span class="tex-span"><i>m</i></span> lines contain description of queries. <span class="tex-span"><i>i</i></span>&nbsp;-th line (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>m</i></span>) describes the <span class="tex-span"><i>i</i></span>&nbsp;-th level and contains an integer <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— the index of the parent-class of class with index <span class="tex-span"><i>i</i> + 1</span> (<span class="tex-span">1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>i</i></span>). </p>

## Output

<p>Suppose that at <span class="tex-span"><i>i</i></span>&nbsp;-th level the maximum cost of changing one class to another is <span class="tex-span"><i>x</i></span>. For each level output the number of classes such that for each of these classes there exists some other class <span class="tex-span"><i>y</i></span>, and the distance from this class to <span class="tex-span"><i>y</i></span> is exactly <span class="tex-span"><i>x</i></span>.</p>





```input1
4
1
1
2
1

```




```input2
4
1
1
2
3

```




```output1
2
2
2
3

```




```output2
2
2
2
2

```


