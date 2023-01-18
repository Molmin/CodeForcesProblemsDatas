## Description

<div><center> <img class="tex-graphics" src="file://ZoitJe30.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Slastyona likes to watch life of nearby grove's dwellers. This time she watches a strange red-black spider sitting at the center of a huge cobweb.</p><p>The cobweb is a set of <span class="tex-span"><i>n</i></span> nodes connected by threads, each of the treads is either red of black. Using these threads, the spider can move between nodes. No thread connects a node to itself, and between any two nodes there is a unique sequence of threads connecting them.</p><p>Slastyona decided to study some special qualities of the cobweb. She noticed that each of the threads has a value of <span class="tex-font-style-it">clamminess</span> <span class="tex-span"><i>x</i></span>.</p><p>However, Slastyona is mostly interested in <span class="tex-font-style-it">jelliness</span> of the cobweb. Consider those of the shortest paths between each pair of nodes on which the numbers of red and black threads differ at most twice. For each such path compute the product of the clamminess of threads on the path.The jelliness of the cobweb is the product of all obtained values among all paths. Those paths that differ by direction only are counted only once.</p><p>Of course, this number can be huge, so Slastyona asks you to compute the jelliness of the given cobweb and print the answer modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line contains the number of nodes <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p><p>The next <span class="tex-span"><i>n</i> - 1</span> lines contain four integers each, denoting the <span class="tex-span"><i>i</i></span>-th thread of the cobweb: the nodes it connects <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>, the <span class="tex-font-style-it">clamminess</span> of the thread <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup> + 6)</span>, and the color of the thread <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<img align="middle" class="tex-formula" src="file://yDUBWWpk.png" style="max-width: 100.0%;max-height: 100.0%;">). The red color is denoted by <span class="tex-span">0</span>, and the black color is denoted by <span class="tex-span">1</span>. </p></div><div class="output-specification"><p>Print single integer the <span class="tex-font-style-it">jelliness</span> of the cobweb modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>. If there are no paths such that the numbers of red and black threads differ at most twice, print <span class="tex-span">1</span>.</p></div>

## Input

<p>The first line contains the number of nodes <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p><p>The next <span class="tex-span"><i>n</i> - 1</span> lines contain four integers each, denoting the <span class="tex-span"><i>i</i></span>-th thread of the cobweb: the nodes it connects <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>, the <span class="tex-font-style-it">clamminess</span> of the thread <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup> + 6)</span>, and the color of the thread <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<img align="middle" class="tex-formula" src="file://yDUBWWpk.png" style="max-width: 100.0%;max-height: 100.0%;">). The red color is denoted by <span class="tex-span">0</span>, and the black color is denoted by <span class="tex-span">1</span>. </p>

## Output

<p>Print single integer the <span class="tex-font-style-it">jelliness</span> of the cobweb modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>. If there are no paths such that the numbers of red and black threads differ at most twice, print <span class="tex-span">1</span>.</p>





```input1
5
1 2 9 0
2 3 5 1
2 4 5 0
2 5 5 1

```




```input2
8
1 2 7 1
2 3 4 1
3 4 19 1
5 1 2 0
6 2 3 0
7 3 3 0
8 4 4 0

```




```output1
1265625

```




```output2
452841614

```



## Note

<p>In the first example there are <span class="tex-span">4</span> pairs of nodes such that the numbers of threads of both colors on them differ at most twice. There pairs are <span class="tex-span">(1, 3)</span> with product of clamminess equal to <span class="tex-span">45</span>, <span class="tex-span">(1, 5)</span> with product of clamminess equal to <span class="tex-span">45</span>, <span class="tex-span">(3, 4)</span> with product of clamminess equal to <span class="tex-span">25</span> and <span class="tex-span">(4, 5)</span> with product of clamminess equal to <span class="tex-span">25</span>. The <span class="tex-font-style-it">jelliness</span> of the cobweb is equal to 1265625.</p>
