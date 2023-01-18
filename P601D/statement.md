## Description

<div><p>You are given a tree <span class="tex-span"><i>T</i></span> with <span class="tex-span"><i>n</i></span> vertices (numbered <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span>) and a letter in each vertex. The tree is rooted at vertex <span class="tex-span">1</span>.</p><p>Let's look at the subtree <span class="tex-span"><i>T</i><sub class="lower-index"><i>v</i></sub></span> of some vertex <span class="tex-span"><i>v</i></span>. It is possible to read a string along each simple path starting at <span class="tex-span"><i>v</i></span> and ending at some vertex in <span class="tex-span"><i>T</i><sub class="lower-index"><i>v</i></sub></span> (possibly <span class="tex-span"><i>v</i></span> itself). Let's denote the number of <span class="tex-font-style-bf">distinct</span> strings which can be read this way as <img align="middle" class="tex-formula" src="file://IYJ2LKeg.png" style="max-width: 100.0%;max-height: 100.0%;">. </p><p>Also, there's a number <span class="tex-span"><i>c</i><sub class="lower-index"><i>v</i></sub></span> assigned to each vertex <span class="tex-span"><i>v</i></span>. We are interested in vertices with the maximum value of <img align="middle" class="tex-formula" src="file://kLcN9b5L.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>You should compute two statistics: the maximum value of <img align="middle" class="tex-formula" src="file://n9kQJXcd.png" style="max-width: 100.0%;max-height: 100.0%;"> and the number of vertices <span class="tex-span"><i>v</i></span> with the maximum <img align="middle" class="tex-formula" src="file://QX68ms1H.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div><div class="input-specification"><p>The first line of the input contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300 000</span>)&nbsp;— the number of vertices of the tree.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The third line contains a string <span class="tex-span"><i>s</i></span> consisting of <span class="tex-span"><i>n</i></span> lowercase English letters&nbsp;— the <span class="tex-span"><i>i</i></span>-th character of this string is the letter in vertex <span class="tex-span"><i>i</i></span>.</p><p>The following <span class="tex-span"><i>n</i> - 1</span> lines describe the tree <span class="tex-span"><i>T</i></span>. Each of them contains two space-separated integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>) indicating an edge between vertices <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>.</p><p>It's guaranteed that the input will describe a tree.</p></div><div class="output-specification"><p>Print two lines. </p><p>On the first line, print <img align="middle" class="tex-formula" src="file://WBVCxfO5.png" style="max-width: 100.0%;max-height: 100.0%;"> over all <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>. </p><p>On the second line, print the number of vertices <span class="tex-span"><i>v</i></span> for which <img align="middle" class="tex-formula" src="file://teWxrzyX.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line of the input contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300 000</span>)&nbsp;— the number of vertices of the tree.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The third line contains a string <span class="tex-span"><i>s</i></span> consisting of <span class="tex-span"><i>n</i></span> lowercase English letters&nbsp;— the <span class="tex-span"><i>i</i></span>-th character of this string is the letter in vertex <span class="tex-span"><i>i</i></span>.</p><p>The following <span class="tex-span"><i>n</i> - 1</span> lines describe the tree <span class="tex-span"><i>T</i></span>. Each of them contains two space-separated integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>) indicating an edge between vertices <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>.</p><p>It's guaranteed that the input will describe a tree.</p>

## Output

<p>Print two lines. </p><p>On the first line, print <img align="middle" class="tex-formula" src="file://WBVCxfO5.png" style="max-width: 100.0%;max-height: 100.0%;"> over all <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>. </p><p>On the second line, print the number of vertices <span class="tex-span"><i>v</i></span> for which <img align="middle" class="tex-formula" src="file://teWxrzyX.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
10
1 2 7 20 20 30 40 50 50 50
cacabbcddd
1 2
6 8
7 2
6 2
5 4
5 9
3 10
2 5
2 3

```




```input2
6
0 2 4 1 1 1
raaaba
1 2
2 3
2 4
2 5
3 6

```




```output1
51
3

```




```output2
6
2

```



## Note

<p>In the first sample, the tree looks like this:</p><center> <img class="tex-graphics" src="file://P1NGOYo9.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The sets of strings that can be read from individual vertices are:</p><center> <img class="tex-graphics" src="file://jUWs0Bc8.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Finally, the values of <img align="middle" class="tex-formula" src="file://nGaZI0wX.png" style="max-width: 100.0%;max-height: 100.0%;"> are:</p><center> <img class="tex-graphics" src="file://wNdImspe.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second sample, the values of <img align="middle" class="tex-formula" src="file://QHnPuDrw.png" style="max-width: 100.0%;max-height: 100.0%;"> are <span class="tex-span">(5, 4, 2, 1, 1, 1)</span>. The distinct strings read in <span class="tex-span"><i>T</i><sub class="lower-index">2</sub></span> are <img align="middle" class="tex-formula" src="file://BdCheUWY.png" style="max-width: 100.0%;max-height: 100.0%;">; note that <img align="middle" class="tex-formula" src="file://Jz4cQnwV.png" style="max-width: 100.0%;max-height: 100.0%;"> can be read down to vertices <span class="tex-span">3</span> or <span class="tex-span">4</span>.</p>
