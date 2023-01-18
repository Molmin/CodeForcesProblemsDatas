## Description

<div><p><span class="tex-font-style-it">"Eat a beaver, save a tree!" — That will be the motto of ecologists' urgent meeting in Beaverley Hills.</span></p><p><span class="tex-font-style-it">And the whole point is that the population of beavers on the Earth has reached incredible sizes! Each day their number increases in several times and they don't even realize how much their unhealthy obsession with trees harms the nature and the humankind. The amount of oxygen in the atmosphere has dropped to 17 per cent and, as the best minds of the world think, that is not the end.</span></p><p><span class="tex-font-style-it">In the middle of the 50-s of the previous century a group of soviet scientists succeed in foreseeing the situation with beavers and worked out a secret technology to clean territory. The technology bears a mysterious title "Beavermuncher-0xFF". Now the fate of the planet lies on the fragile shoulders of a small group of people who has dedicated their lives to science.</span></p><p><span class="tex-font-style-it">The prototype is ready, you now need to urgently carry out its experiments in practice.</span> </p><p>You are given a tree, completely occupied by beavers. A tree is a connected undirected graph without cycles. The tree consists of <span class="tex-span"><i>n</i></span> vertices, the <span class="tex-span"><i>i</i></span>-th vertex contains <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> beavers. </p><p>"Beavermuncher-0xFF" works by the following principle: being at some vertex <span class="tex-span"><i>u</i></span>, it can go to the vertex <span class="tex-span"><i>v</i></span>, if they are connected by an edge, and eat <span class="tex-font-style-bf">exactly one</span> beaver located at the vertex <span class="tex-span"><i>v</i></span>. It is impossible to move to the vertex <span class="tex-span"><i>v</i></span> if there are no beavers left in <span class="tex-span"><i>v</i></span>. "Beavermuncher-0xFF" <span class="tex-font-style-bf">cannot</span> just stand at some vertex and eat beavers in it. "Beavermuncher-0xFF" must move without stops.</p><p>Why does the "Beavermuncher-0xFF" works like this? Because the developers have not provided place for the battery in it and eating beavers is necessary for converting their mass into pure energy.</p><p>It is guaranteed that the beavers will be shocked by what is happening, which is why they will not be able to move from a vertex of the tree to another one. As for the "Beavermuncher-0xFF", it can move along each edge in both directions while conditions described above are fulfilled.</p><p>The root of the tree is located at the vertex <span class="tex-span"><i>s</i></span>. This means that the "Beavermuncher-0xFF" begins its mission at the vertex <span class="tex-span"><i>s</i></span> and it must return there at the end of experiment, because no one is going to take it down from a high place. </p><p>Determine the maximum number of beavers "Beavermuncher-0xFF" can eat and return to the starting vertex.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> — the number of vertices in the tree (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) — amounts of beavers on corresponding vertices. Following <span class="tex-span"><i>n</i> - 1</span> lines describe the tree. Each line contains two integers separated by space. These integers represent two vertices connected by an edge. Vertices are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The last line contains integer <span class="tex-span"><i>s</i></span> — the number of the starting vertex (<span class="tex-span">1 ≤ <i>s</i> ≤ <i>n</i></span>).</p></div><div class="output-specification"><p>Print the maximum number of beavers munched by the "Beavermuncher-0xFF".</p><p>Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to write 64-bit integers in C++. It is preferred to use <span class="tex-font-style-tt">cout</span> (also you may use <span class="tex-font-style-tt">%I64d</span>).</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> — the number of vertices in the tree (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) — amounts of beavers on corresponding vertices. Following <span class="tex-span"><i>n</i> - 1</span> lines describe the tree. Each line contains two integers separated by space. These integers represent two vertices connected by an edge. Vertices are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The last line contains integer <span class="tex-span"><i>s</i></span> — the number of the starting vertex (<span class="tex-span">1 ≤ <i>s</i> ≤ <i>n</i></span>).</p>

## Output

<p>Print the maximum number of beavers munched by the "Beavermuncher-0xFF".</p><p>Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to write 64-bit integers in C++. It is preferred to use <span class="tex-font-style-tt">cout</span> (also you may use <span class="tex-font-style-tt">%I64d</span>).</p>





```input1
5
1 3 1 3 2
2 5
3 4
4 5
1 5
4

```




```input2
3
2 1 1
3 2
1 2
3

```




```output1
6

```




```output2
2

```


