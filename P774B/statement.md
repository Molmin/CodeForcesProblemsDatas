## Description

<div><p>Stepan is a very experienced olympiad participant. He has <span class="tex-span"><i>n</i></span> cups for Physics olympiads and <span class="tex-span"><i>m</i></span> cups for Informatics olympiads. Each cup is characterized by two parameters — its significance <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and width <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Stepan decided to expose some of his cups on a shelf with width <span class="tex-span"><i>d</i></span> in such a way, that:</p><ul> <li> there is at least one Physics cup and at least one Informatics cup on the shelf, </li><li> the total width of the exposed cups does not exceed <span class="tex-span"><i>d</i></span>, </li><li> from each subjects (Physics and Informatics) some of the most significant cups are exposed (i. e. if a cup for some subject with significance <span class="tex-span"><i>x</i></span> is exposed, then all the cups for this subject with significance greater than <span class="tex-span"><i>x</i></span> must be exposed too). </li></ul><p>Your task is to determine the maximum possible total significance, which Stepan can get when he exposes cups on the shelf with width <span class="tex-span"><i>d</i></span>, considering all the rules described above. The total significance is the sum of significances of all the exposed cups.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>d</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of cups for Physics olympiads, the number of cups for Informatics olympiads and the width of the shelf.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — significance and width of the <span class="tex-span"><i>i</i></span>-th cup for Physics olympiads.</p><p>Each of the following <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>j</i></sub>, <i>w</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — significance and width of the <span class="tex-span"><i>j</i></span>-th cup for Informatics olympiads.</p></div><div class="output-specification"><p>Print the maximum possible total significance, which Stepan can get exposing cups on the shelf with width <span class="tex-span"><i>d</i></span>, considering all the rules described in the statement.</p><p>If there is no way to expose cups on the shelf, then print <span class="tex-span">0</span>.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>d</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of cups for Physics olympiads, the number of cups for Informatics olympiads and the width of the shelf.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — significance and width of the <span class="tex-span"><i>i</i></span>-th cup for Physics olympiads.</p><p>Each of the following <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>j</i></sub>, <i>w</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — significance and width of the <span class="tex-span"><i>j</i></span>-th cup for Informatics olympiads.</p>

## Output

<p>Print the maximum possible total significance, which Stepan can get exposing cups on the shelf with width <span class="tex-span"><i>d</i></span>, considering all the rules described in the statement.</p><p>If there is no way to expose cups on the shelf, then print <span class="tex-span">0</span>.</p>





```input1
3 1 8
4 2
5 5
4 2
3 2

```




```input2
4 3 12
3 4
2 4
3 5
3 4
3 5
5 2
3 4

```




```input3
2 2 2
5 3
6 3
4 2
8 1

```




```output1
8

```




```output2
11

```




```output3
0

```



## Note

<p>In the first example Stepan has only one Informatics cup which must be exposed on the shelf. Its significance equals <span class="tex-span">3</span> and width equals <span class="tex-span">2</span>, so after Stepan exposes it, the width of free space on the shelf becomes equal to <span class="tex-span">6</span>. Also, Stepan must expose the second Physics cup (which has width <span class="tex-span">5</span>), because it is the most significant cup for Physics (its significance equals <span class="tex-span">5</span>). After that Stepan can not expose more cups on the shelf, because there is no enough free space. Thus, the maximum total significance of exposed cups equals to <span class="tex-span">8</span>.</p>
