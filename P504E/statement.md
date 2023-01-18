## Description

<div><p>Misha has a tree with characters written on the vertices. He can choose two vertices <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> of this tree and write down characters of vertices lying on a path from <span class="tex-span"><i>s</i></span> to <span class="tex-span"><i>t</i></span>. We'll say that such string corresponds to pair <span class="tex-span">(<i>s</i>, <i>t</i>)</span>.</p><p>Misha has <span class="tex-span"><i>m</i></span> queries of type: you are given <span class="tex-span">4</span> vertices <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span>, <span class="tex-span"><i>d</i></span>; you need to find the largest common prefix of the strings that correspond to pairs <span class="tex-span">(<i>a</i>, <i>b</i>)</span> and <span class="tex-span">(<i>c</i>, <i>d</i>)</span>. Your task is to help him.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300 000</span>) — the number of vertices in the tree.</p><p>Next follows a line consisting of <span class="tex-span"><i>n</i></span> small English letters. The <span class="tex-span"><i>i</i></span>-th character of the string corresponds to the character written on the <span class="tex-span"><i>i</i></span>-th vertex. </p><p>Next <span class="tex-span"><i>n</i> - 1</span> lines contain information about edges. An edge is defined by a pair of integers <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i> ≠ <i>v</i></span>), separated by spaces.</p><p>The next line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 1 000 000</span>) — the number of queries.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain information about queries. A query is defined by four integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span>, <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>c</i>, <i>d</i> ≤ <i>n</i></span>), separated by spaces.</p></div><div class="output-specification"><p>For each query print the length of the largest common prefix on a separate line.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300 000</span>) — the number of vertices in the tree.</p><p>Next follows a line consisting of <span class="tex-span"><i>n</i></span> small English letters. The <span class="tex-span"><i>i</i></span>-th character of the string corresponds to the character written on the <span class="tex-span"><i>i</i></span>-th vertex. </p><p>Next <span class="tex-span"><i>n</i> - 1</span> lines contain information about edges. An edge is defined by a pair of integers <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i> ≠ <i>v</i></span>), separated by spaces.</p><p>The next line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 1 000 000</span>) — the number of queries.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain information about queries. A query is defined by four integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span>, <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>c</i>, <i>d</i> ≤ <i>n</i></span>), separated by spaces.</p>

## Output

<p>For each query print the length of the largest common prefix on a separate line.</p>





```input1
6
bbbabb
2 1
3 2
4 3
5 2
6 5
6
2 5 3 1
1 5 2 3
5 6 5 6
6 3 4 1
6 2 3 4
2 2 4 5

```




```output1
2
2
2
0
1
0

```


