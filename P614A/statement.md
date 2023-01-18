## Description

<div><p>Programmer Rostislav got seriously interested in the Link/Cut Tree data structure, which is based on Splay trees. Specifically, he is now studying the <span class="tex-span"><i>expose</i></span> procedure.</p><p>Unfortunately, Rostislav is unable to understand the definition of this procedure, so he decided to ask programmer Serezha to help him. Serezha agreed to help if Rostislav solves a simple task (and if he doesn't, then why would he need Splay trees anyway?)</p><p>Given integers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>k</i></span>, you need to print all powers of number <span class="tex-span"><i>k</i></span> within range from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span> <span class="tex-font-style-bf">inclusive</span>. However, Rostislav doesn't want to spent time doing this, as he got interested in playing a network game called Agar with Gleb. Help him!</p></div><div class="input-specification"><p>The first line of the input contains three space-separated integers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span">2 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print all powers of number <span class="tex-span"><i>k</i></span>, that lie within range from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span> in the increasing order. If there are no such numbers, print "<span class="tex-font-style-tt">-1</span>" (without the quotes).</p></div>

## Input

<p>The first line of the input contains three space-separated integers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span">2 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print all powers of number <span class="tex-span"><i>k</i></span>, that lie within range from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span> in the increasing order. If there are no such numbers, print "<span class="tex-font-style-tt">-1</span>" (without the quotes).</p>





```input1
1 10 2

```




```input2
2 4 5

```




```output1
1 2 4 8
```




```output2
-1
```



## Note

<p>Note to the first sample: numbers <span class="tex-span">2<sup class="upper-index">0</sup> = 1</span>, <span class="tex-span">2<sup class="upper-index">1</sup> = 2</span>, <span class="tex-span">2<sup class="upper-index">2</sup> = 4</span>, <span class="tex-span">2<sup class="upper-index">3</sup> = 8</span> lie within the specified range. The number <span class="tex-span">2<sup class="upper-index">4</sup> = 16</span> is greater then <span class="tex-span">10</span>, thus it shouldn't be printed.</p>
