## Description

<div><p>While learning Computational Geometry, Tiny is simultaneously learning a useful data structure called segment tree or interval tree. He has scarcely grasped it when comes out a strange problem:</p><p>Given an integer sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. You should run <span class="tex-span"><i>q</i></span> queries of two types:</p><ol> <li> Given two integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>), ask the sum of all elements in the sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i></sub>, <i>a</i><sub class="lower-index"><i>l</i> + 1</sub>, ..., <i>a</i><sub class="lower-index"><i>r</i></sub></span>. </li><li> Given two integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>), let each element <span class="tex-span"><i>x</i></span> in the sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i></sub>, <i>a</i><sub class="lower-index"><i>l</i> + 1</sub>, ..., <i>a</i><sub class="lower-index"><i>r</i></sub></span> becomes <span class="tex-span"><i>x</i><sup class="upper-index">3</sup></span>. In other words, apply an assignments <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i></sub> = <i>a</i><sub class="lower-index"><i>l</i></sub><sup class="upper-index">3</sup>, <i>a</i><sub class="lower-index"><i>l</i> + 1</sub> = <i>a</i><sub class="lower-index"><i>l</i> + 1</sub><sup class="upper-index">3</sup>, ..., <i>a</i><sub class="lower-index"><i>r</i></sub> = <i>a</i><sub class="lower-index"><i>r</i></sub><sup class="upper-index">3</sup></span>. </li></ol><p>For every query of type 1, output the answer to it.</p><p>Tiny himself surely cannot work it out, so he asks you for help. In addition, Tiny is a prime lover. He tells you that because the answer may be too huge, you should only output it modulo <span class="tex-span">95542721</span> (this number is a prime number).</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), representing the length of the sequence. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The third line contains an integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>), representing the number of queries. Then follow <span class="tex-span"><i>q</i></span> lines. Each line contains three integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>), <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> stands for the type of the query while <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> is the parameters of the query, correspondingly.</p></div><div class="output-specification"><p>For each 1-type query, print the answer to it per line.</p><p>You should notice that each printed number should be non-negative and less than <span class="tex-span">95542721</span>.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), representing the length of the sequence. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The third line contains an integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>), representing the number of queries. Then follow <span class="tex-span"><i>q</i></span> lines. Each line contains three integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>), <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> stands for the type of the query while <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> is the parameters of the query, correspondingly.</p>

## Output

<p>For each 1-type query, print the answer to it per line.</p><p>You should notice that each printed number should be non-negative and less than <span class="tex-span">95542721</span>.</p>





```input1
8
1 2 3 4 5 6 7 8
5
1 2 5
2 2 5
1 2 5
2 3 6
1 4 7

```




```output1
14
224
2215492

```


