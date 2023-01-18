## Description

<div><p>Yet another round on DecoForces is coming! Grandpa Maks wanted to participate in it but someone has stolen his precious sofa! And how can one perform well with such a major loss?</p><p>Fortunately, the thief had left a note for Grandpa Maks. This note got Maks to the sofa storehouse. Still he had no idea which sofa belongs to him as they all looked the same!</p><p>The storehouse is represented as matrix <span class="tex-span"><i>n</i> × <i>m</i></span>. Every sofa takes two neighbouring by some side cells. No cell is covered by more than one sofa. There can be empty cells.</p><p>Sofa <span class="tex-span"><i>A</i></span> is standing to the left of sofa <span class="tex-span"><i>B</i></span> if there exist two such cells <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> that <span class="tex-font-style-bf"><span class="tex-span"><i>x</i><sub class="lower-index"><i>a</i></sub> &lt; <i>x</i><sub class="lower-index"><i>b</i></sub></span></span>, <span class="tex-span"><i>a</i></span> is covered by <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>b</i></span> is covered by <span class="tex-span"><i>B</i></span>. Sofa <span class="tex-span"><i>A</i></span> is standing to the top of sofa <span class="tex-span"><i>B</i></span> if there exist two such cells <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> that <span class="tex-font-style-bf"><span class="tex-span"><i>y</i><sub class="lower-index"><i>a</i></sub> &lt; <i>y</i><sub class="lower-index"><i>b</i></sub></span></span>, <span class="tex-span"><i>a</i></span> is covered by <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>b</i></span> is covered by <span class="tex-span"><i>B</i></span>. Right and bottom conditions are declared the same way. </p><p><span class="tex-font-style-bf">Note that in all conditions <span class="tex-span"><i>A</i> ≠ <i>B</i></span>.</span> Also some sofa <span class="tex-span"><i>A</i></span> can be both to the top of another sofa <span class="tex-span"><i>B</i></span> and to the bottom of it. The same is for left and right conditions.</p><p>The note also stated that there are <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>l</i></sub></span> sofas to the left of Grandpa Maks's sofa, <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>r</i></sub></span> — to the right, <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>t</i></sub></span> — to the top and <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>b</i></sub></span> — to the bottom.</p><p>Grandpa Maks asks you to help him to identify his sofa. It is guaranteed that there is no more than one sofa of given conditions.</p><p>Output the number of Grandpa Maks's sofa. If there is no such sofa that all the conditions are met for it then output <span class="tex-font-style-tt">-1</span>.</p></div><div class="input-specification"><p>The first line contains one integer number <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>d</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of sofas in the storehouse.</p><p>The second line contains two integer numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the size of the storehouse.</p><p>Next <span class="tex-span"><i>d</i></span> lines contains four integer numbers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub> ≤ <i>m</i></span>) — coordinates of the <span class="tex-span"><i>i</i></span>-th sofa. It is guaranteed that cells (<span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub></span>) and (<span class="tex-span"><i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span>) have common side, (<span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub></span>) <span class="tex-span"> ≠ </span> (<span class="tex-span"><i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span>) and no cell is covered by more than one sofa.</p><p>The last line contains four integer numbers <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>l</i></sub></span>, <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>r</i></sub></span>, <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>t</i></sub></span>, <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>b</i></sub></span> (<span class="tex-span">0 ≤ <i>cnt</i><sub class="lower-index"><i>l</i></sub>, <i>cnt</i><sub class="lower-index"><i>r</i></sub>, <i>cnt</i><sub class="lower-index"><i>t</i></sub>, <i>cnt</i><sub class="lower-index"><i>b</i></sub> ≤ <i>d</i> - 1</span>).</p></div><div class="output-specification"><p>Print the number of the sofa for which all the conditions are met. Sofas are numbered <span class="tex-span">1</span> through <span class="tex-span"><i>d</i></span> as given in input. If there is no such sofa then print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains one integer number <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>d</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of sofas in the storehouse.</p><p>The second line contains two integer numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the size of the storehouse.</p><p>Next <span class="tex-span"><i>d</i></span> lines contains four integer numbers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub> ≤ <i>m</i></span>) — coordinates of the <span class="tex-span"><i>i</i></span>-th sofa. It is guaranteed that cells (<span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub></span>) and (<span class="tex-span"><i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span>) have common side, (<span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub></span>) <span class="tex-span"> ≠ </span> (<span class="tex-span"><i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span>) and no cell is covered by more than one sofa.</p><p>The last line contains four integer numbers <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>l</i></sub></span>, <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>r</i></sub></span>, <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>t</i></sub></span>, <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>b</i></sub></span> (<span class="tex-span">0 ≤ <i>cnt</i><sub class="lower-index"><i>l</i></sub>, <i>cnt</i><sub class="lower-index"><i>r</i></sub>, <i>cnt</i><sub class="lower-index"><i>t</i></sub>, <i>cnt</i><sub class="lower-index"><i>b</i></sub> ≤ <i>d</i> - 1</span>).</p>

## Output

<p>Print the number of the sofa for which all the conditions are met. Sofas are numbered <span class="tex-span">1</span> through <span class="tex-span"><i>d</i></span> as given in input. If there is no such sofa then print <span class="tex-font-style-tt">-1</span>.</p>





```input1
2
3 2
3 1 3 2
1 2 2 2
1 0 0 1

```




```input2
3
10 10
1 2 1 1
5 5 6 5
6 4 5 4
2 1 2 0

```




```input3
2
2 2
2 1 1 1
1 2 2 2
1 0 0 0

```




```output1
1

```




```output2
2

```




```output3
-1

```



## Note

<p>Let's consider the second example. </p><ul> <li> The first sofa has <span class="tex-span">0</span> to its left, <span class="tex-span">2</span> sofas to its right (<span class="tex-span">(1, 1)</span> is to the left of both <span class="tex-span">(5, 5)</span> and <span class="tex-span">(5, 4)</span>), <span class="tex-span">0</span> to its top and <span class="tex-span">2</span> to its bottom (both <span class="tex-span">2</span>nd and <span class="tex-span">3</span>rd sofas are below). </li><li> The second sofa has <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>l</i></sub> = 2</span>, <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>r</i></sub> = 1</span>, <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>t</i></sub> = 2</span> and <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>b</i></sub> = 0</span>. </li><li> The third sofa has <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>l</i></sub> = 2</span>, <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>r</i></sub> = 1</span>, <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>t</i></sub> = 1</span> and <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>b</i></sub> = 1</span>. </li></ul><p>So the second one corresponds to the given conditions.</p><p>In the third example </p><ul> <li> The first sofa has <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>l</i></sub> = 1</span>, <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>r</i></sub> = 1</span>, <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>t</i></sub> = 0</span> and <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>b</i></sub> = 1</span>. </li><li> The second sofa has <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>l</i></sub> = 1</span>, <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>r</i></sub> = 1</span>, <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>t</i></sub> = 1</span> and <span class="tex-span"><i>cnt</i><sub class="lower-index"><i>b</i></sub> = 0</span>. </li></ul><p>And there is no sofa with the set <span class="tex-span">(1, 0, 0, 0)</span> so the answer is <span class="tex-font-style-tt">-1</span>.</p>
