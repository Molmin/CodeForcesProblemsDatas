## Description

<div><p>In this problem you have to implement an algorithm to defragment your hard disk. The hard disk consists of a sequence of clusters, numbered by integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The disk has <span class="tex-span"><i>m</i></span> recorded files, the <span class="tex-span"><i>i</i></span>-th file occupies clusters with numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, 1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, 2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>n</i><sub class="lower-index"><i>i</i></sub></sub></span>. These clusters are not necessarily located consecutively on the disk, but the order in which they are given corresponds to their sequence in the file (cluster <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, 1</sub></span> contains the first fragment of the <span class="tex-span"><i>i</i></span>-th file, cluster <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, 2</sub></span> has the second fragment, etc.). Also the disc must have one or several clusters which are free from files.</p><p>You are permitted to perform operations of copying the contents of cluster number <span class="tex-span"><i>i</i></span> to cluster number <span class="tex-span"><i>j</i></span> (<span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> must be different). Moreover, if the cluster number <span class="tex-span"><i>j</i></span> used to keep some information, it is lost forever. Clusters are not cleaned, but after the defragmentation is complete, some of them are simply declared unusable (although they may possibly still contain some fragments of files).</p><p>Your task is to use a sequence of copy operations to ensure that each file occupies a contiguous area of memory. Each file should occupy a consecutive cluster section, the files must follow one after another from the beginning of the hard disk. After defragmentation all free (unused) clusters should be at the end of the hard disk. After defragmenting files can be placed in an arbitrary order. Clusters of each file should go consecutively from first to last. See explanatory examples in the notes.</p><p>Print the sequence of operations leading to the disk defragmentation. Note that <span class="tex-font-style-bf">you do not have to minimize</span> the number of operations, but it should not exceed <span class="tex-span">2<i>n</i></span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 200</span>) — the number of clusters and the number of files, correspondingly. Next <span class="tex-span"><i>m</i></span> lines contain descriptions of the files. The first number in the line is <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub> ≥ 1</span>), the number of clusters occupied by the <span class="tex-span"><i>i</i></span>-th file. Then follow <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, 1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, 2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>n</i><sub class="lower-index"><i>i</i></sub></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ <i>n</i></span>). It is guaranteed that each cluster number occurs not more than once and <img align="middle" class="tex-formula" src="file://JuhGJi53.png" style="max-width: 100.0%;max-height: 100.0%;">, that is, there exists at least one unused cluster. Numbers on each line are separated by spaces. </p></div><div class="output-specification"><p>In the first line print a single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 2<i>n</i></span>) — the number of operations needed to defragment the disk. Next <span class="tex-span"><i>k</i></span> lines should contain the operations' descriptions as "<span class="tex-span"><i>i</i></span> <span class="tex-span"><i>j</i></span>" (copy the contents of the cluster number <span class="tex-span"><i>i</i></span> to the cluster number <span class="tex-span"><i>j</i></span>). </p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 200</span>) — the number of clusters and the number of files, correspondingly. Next <span class="tex-span"><i>m</i></span> lines contain descriptions of the files. The first number in the line is <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub> ≥ 1</span>), the number of clusters occupied by the <span class="tex-span"><i>i</i></span>-th file. Then follow <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, 1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, 2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>n</i><sub class="lower-index"><i>i</i></sub></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ <i>n</i></span>). It is guaranteed that each cluster number occurs not more than once and <img align="middle" class="tex-formula" src="file://JuhGJi53.png" style="max-width: 100.0%;max-height: 100.0%;">, that is, there exists at least one unused cluster. Numbers on each line are separated by spaces. </p>

## Output

<p>In the first line print a single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 2<i>n</i></span>) — the number of operations needed to defragment the disk. Next <span class="tex-span"><i>k</i></span> lines should contain the operations' descriptions as "<span class="tex-span"><i>i</i></span> <span class="tex-span"><i>j</i></span>" (copy the contents of the cluster number <span class="tex-span"><i>i</i></span> to the cluster number <span class="tex-span"><i>j</i></span>). </p>





```input1
7 2
2 1 2
3 3 4 5

```




```input2
7 2
2 1 3
3 2 4 5

```




```output1
0

```




```output2
3
2 6
3 2
6 3

```



## Note

<p>Let's say that a disk consists of <span class="tex-span">8</span> clusters and contains two files. The first file occupies two clusters and the second file occupies three clusters. Let's look at examples of correct and incorrect positions of files after defragmentation. </p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://CBVUZ15q.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>Example 2: each file must occupy a contiguous area of memory.</p><p>Example 3: the order of files to each other is not important, at first the second file can be written, and then — the first one.</p><p>Example 4: violating the order of file fragments to each other is not allowed.</p><p>Example 5: unused clusters should be located at the end, and in this example the unused clusters are <span class="tex-span">3</span>, <span class="tex-span">7</span>, <span class="tex-span">8</span>.</p>
