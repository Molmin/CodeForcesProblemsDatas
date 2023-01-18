## Description

<div><p>Duff is the queen of her country, Andarz Gu. She's a competitive programming fan. That's why, when he saw her minister, Malek, free, she gave her a sequence consisting of <span class="tex-span"><i>n</i></span> non-negative integers, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> and asked him to perform <span class="tex-span"><i>q</i></span> queries for her on this sequence.</p><center> <img class="tex-graphics" src="file://hGbxJMxS.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>There are two types of queries:</p><ol> <li> given numbers <span class="tex-span"><i>l</i>, <i>r</i></span> and <span class="tex-span"><i>k</i></span>, Malek should perform <img align="middle" class="tex-formula" src="file://OWVVhfqg.png" style="max-width: 100.0%;max-height: 100.0%;"> for each <span class="tex-span"><i>l</i> ≤ <i>i</i> ≤ <i>r</i></span> (<img align="middle" class="tex-formula" src="file://j1W2LPTm.png" style="max-width: 100.0%;max-height: 100.0%;">, bitwise exclusive OR of numbers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>). </li><li> given numbers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> Malek should tell her the score of sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i></sub>, <i>a</i><sub class="lower-index"><i>l</i> + 1</sub>, ... , <i>a</i><sub class="lower-index"><i>r</i></sub></span>. </li></ol><p>Score of a sequence <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, ..., <i>b</i><sub class="lower-index"><i>k</i></sub></span> is the number of its different Kheshtaks. A non-negative integer <span class="tex-span"><i>w</i></span> is a Kheshtak of this sequence if and only if there exists a subsequence of <span class="tex-span"><i>b</i></span>, let's denote it as <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i><sub class="lower-index">1</sub></sub>, <i>b</i><sub class="lower-index"><i>i</i><sub class="lower-index">2</sub></sub>, ... , <i>b</i><sub class="lower-index"><i>i</i><sub class="lower-index"><i>x</i></sub></sub></span> (possibly empty) such that <img align="middle" class="tex-formula" src="file://sMzbDdeh.png" style="max-width: 100.0%;max-height: 100.0%;"> (<span class="tex-span">1 ≤ <i>i</i><sub class="lower-index">1</sub> &lt; <i>i</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>i</i><sub class="lower-index"><i>x</i></sub> ≤ <i>k</i></span>). If this subsequence is empty, then <span class="tex-span"><i>w</i> = 0</span>.</p><p>Unlike Duff, Malek is not a programmer. That's why he asked for your help. Please help him perform these queries.</p></div><div class="input-specification"><p>The first line of input contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2 × 10<sup class="upper-index">5</sup></span> and <span class="tex-span">1 ≤ <i>q</i> ≤ 4 × 10<sup class="upper-index">4</sup></span>).</p><p>The second line of input contains <span class="tex-span"><i>n</i></span> integers, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> separated by spaces (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span> for each <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>).</p><p>The next <span class="tex-span"><i>q</i></span> lines contain the queries. Each line starts with an integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 2</span>), type of the corresponding query. If <span class="tex-span"><i>t</i> = 1</span>, then there are three more integers in that line, <span class="tex-span"><i>l</i>, <i>r</i></span> and <span class="tex-span"><i>k</i></span>. Otherwise there are two more integers, <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span>. (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span> and <span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>)</p></div><div class="output-specification"><p>Print the answer of each query of the second type in one line.</p></div>

## Input

<p>The first line of input contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2 × 10<sup class="upper-index">5</sup></span> and <span class="tex-span">1 ≤ <i>q</i> ≤ 4 × 10<sup class="upper-index">4</sup></span>).</p><p>The second line of input contains <span class="tex-span"><i>n</i></span> integers, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> separated by spaces (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span> for each <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>).</p><p>The next <span class="tex-span"><i>q</i></span> lines contain the queries. Each line starts with an integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 2</span>), type of the corresponding query. If <span class="tex-span"><i>t</i> = 1</span>, then there are three more integers in that line, <span class="tex-span"><i>l</i>, <i>r</i></span> and <span class="tex-span"><i>k</i></span>. Otherwise there are two more integers, <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span>. (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span> and <span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>)</p>

## Output

<p>Print the answer of each query of the second type in one line.</p>





```input1
5 5
1 2 3 4 2
2 1 5
1 2 2 8
2 1 5
1 1 3 10
2 2 2

```




```output1
8
16
1

```



## Note

<p>In the first query, we want all Kheshtaks of sequence <span class="tex-span">1, 2, 3, 4, 2</span> which are: <span class="tex-span">0, 1, 2, 3, 4, 5, 6, 7</span>.</p><p>In the third query, we want all Khestaks of sequence <span class="tex-span">1, 10, 3, 4, 2</span> which are: <span class="tex-span">0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15</span>.</p><p>In the fifth query, we want all Kheshtaks of sequence <span class="tex-span">0</span> which is <span class="tex-span">0</span>.</p>
