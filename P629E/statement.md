## Description

<div><p>Famil Door’s City map looks like a tree (undirected connected acyclic graph) so other people call it Treeland. There are <span class="tex-span"><i>n</i></span> intersections in the city connected by <span class="tex-span"><i>n</i> - 1</span> bidirectional roads.</p><p>There are <span class="tex-span"><i>m</i></span> friends of Famil Door living in the city. The <span class="tex-span"><i>i</i></span>-th friend lives at the intersection <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and works at the intersection <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. Everyone in the city is unhappy because there is exactly one simple path between their home and work.</p><p>Famil Door plans to construct exactly one new road and he will randomly choose one among <span class="tex-span"><i>n</i>·(<i>n</i> - 1) / 2</span> possibilities. Note, that he may even build a new road between two cities that are already connected by one.</p><p>He knows, that each of his friends will become happy, if after Famil Door constructs a new road there is a path from this friend home to work and back that doesn't visit the same road twice. Formally, there is a simple cycle containing both <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. </p><p>Moreover, if the friend becomes happy, his pleasure is equal to the length of such path (it's easy to see that it's unique). For each of his friends Famil Door wants to know his expected pleasure, that is the expected length of the cycle containing both <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> if we consider only cases when such a cycle exists.</p></div><div class="input-specification"><p>The first line of the input contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i>,  <i>m</i> ≤ 100 000</span>)&nbsp;— the number of the intersections in the Treeland and the number of Famil Door's friends.</p><p>Then follow <span class="tex-span"><i>n</i> - 1</span> lines describing bidirectional roads. Each of them contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>&nbsp;— the indices of intersections connected by the <span class="tex-span"><i>i</i></span>-th road.</p><p>Last <span class="tex-span"><i>m</i></span> lines of the input describe Famil Door's friends. The <span class="tex-span"><i>i</i></span>-th of these lines contain two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— indices of intersections where the <span class="tex-span"><i>i</i></span>-th friend lives and works.</p></div><div class="output-specification"><p>For each friend you should print the expected value of pleasure if he will be happy. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://vhNgNs9I.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line of the input contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i>,  <i>m</i> ≤ 100 000</span>)&nbsp;— the number of the intersections in the Treeland and the number of Famil Door's friends.</p><p>Then follow <span class="tex-span"><i>n</i> - 1</span> lines describing bidirectional roads. Each of them contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>&nbsp;— the indices of intersections connected by the <span class="tex-span"><i>i</i></span>-th road.</p><p>Last <span class="tex-span"><i>m</i></span> lines of the input describe Famil Door's friends. The <span class="tex-span"><i>i</i></span>-th of these lines contain two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— indices of intersections where the <span class="tex-span"><i>i</i></span>-th friend lives and works.</p>

## Output

<p>For each friend you should print the expected value of pleasure if he will be happy. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://vhNgNs9I.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
4 3
2 4
4 1
3 2
3 1
2 3
4 1

```




```input2
3 3
1 2
1 3
1 2
1 3
2 3

```




```output1
4.00000000
3.00000000
3.00000000

```




```output2
2.50000000
2.50000000
3.00000000

```



## Note

<p>Consider the second sample. </p><ol> <li> Both roads <span class="tex-span">(1, 2)</span> and <span class="tex-span">(2, 3)</span> work, so the expected length if <img align="middle" class="tex-formula" src="file://NhYMKfme.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> Roads <span class="tex-span">(1, 3)</span> and <span class="tex-span">(2, 3)</span> make the second friend happy. Same as for friend <span class="tex-span">1</span> the answer is <span class="tex-span">2.5</span> </li><li> The only way to make the third friend happy is to add road <span class="tex-span">(2, 3)</span>, so the answer is <span class="tex-span">3</span> </li></ol>
