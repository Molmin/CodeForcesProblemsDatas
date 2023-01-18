## Description

<div><p>The Resistance is trying to take control over all planets in a particular solar system. This solar system is shaped like a tree. More precisely, some planets are connected by bidirectional hyperspace tunnels in such a way that there is a path between every pair of the planets, but removing any tunnel would disconnect some of them.</p><p>The Resistance already has measures in place that will, when the time is right, enable them to control every planet that is not <span class="tex-font-style-it">remote</span>. A planet is considered to be remote if it is connected to the rest of the planets only via a single hyperspace tunnel.</p><p>How much work is there left to be done: that is, how many remote planets are there?</p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>N</i></span> (<span class="tex-span">2 ≤ <i>N</i> ≤ 1000</span>) – the number of planets in the galaxy.</p><p>The next <span class="tex-span"><i>N</i> - 1</span> lines describe the hyperspace tunnels between the planets. Each of the <span class="tex-span"><i>N</i> - 1</span> lines contains two space-separated integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>N</i></span>) indicating that there is a bidirectional hyperspace tunnel between the planets <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>. It is guaranteed that every two planets are connected by a path of tunnels, and that each tunnel connects a different pair of planets.</p></div><div class="output-specification"><p>A single integer denoting the number of remote planets.</p></div>

## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>N</i></span> (<span class="tex-span">2 ≤ <i>N</i> ≤ 1000</span>) – the number of planets in the galaxy.</p><p>The next <span class="tex-span"><i>N</i> - 1</span> lines describe the hyperspace tunnels between the planets. Each of the <span class="tex-span"><i>N</i> - 1</span> lines contains two space-separated integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>N</i></span>) indicating that there is a bidirectional hyperspace tunnel between the planets <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>. It is guaranteed that every two planets are connected by a path of tunnels, and that each tunnel connects a different pair of planets.</p>

## Output

<p>A single integer denoting the number of remote planets.</p>





```input1
5
4 1
4 2
1 3
1 5

```




```input2
4
1 2
4 3
1 4

```




```output1
3

```




```output2
2

```



## Note

<p>In the first example, only planets <span class="tex-span">2</span>, <span class="tex-span">3</span> and <span class="tex-span">5</span> are connected by a single tunnel.</p><p>In the second example, the <span class="tex-font-style-it">remote</span> planets are <span class="tex-span">2</span> and <span class="tex-span">3</span>.</p><p>Note that this problem has only two versions – easy and medium.</p>
