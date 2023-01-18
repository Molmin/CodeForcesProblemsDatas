## Description

<div><p>Captain Marmot wants to prepare a huge and important battle against his enemy, Captain Snake. For this battle he has <span class="tex-span"><i>n</i></span> regiments, each consisting of <span class="tex-span">4</span> moles.</p><p>Initially, each mole <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ 4<i>n</i></span>) is placed at some position <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> in the Cartesian plane. Captain Marmot wants to move some moles to make the regiments <span class="tex-font-style-bf">compact</span>, if it's possible.</p><p>Each mole <span class="tex-span"><i>i</i></span> has a home placed at the position <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>)</span>. Moving this mole one time means rotating his position point <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> <span class="tex-span">90</span> degrees counter-clockwise around it's home point <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>)</span>.</p><p>A regiment is <span class="tex-font-style-bf">compact</span> only if the position points of the <span class="tex-span">4</span> moles form a square with non-zero area.</p><p>Help Captain Marmot to find out for each regiment the minimal number of moves required to make that regiment compact, if it's possible.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>), the number of regiments.</p><p>The next <span class="tex-span">4<i>n</i></span> lines contain <span class="tex-span">4</span> integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">4</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>).</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> lines to the standard output. If the regiment <span class="tex-span"><i>i</i></span> can be made compact, the <span class="tex-span"><i>i</i></span>-th line should contain one integer, the minimal number of required moves. Otherwise, on the <span class="tex-span"><i>i</i></span>-th line print <span class="tex-font-style-tt">"-1"</span> (without quotes).</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>), the number of regiments.</p><p>The next <span class="tex-span">4<i>n</i></span> lines contain <span class="tex-span">4</span> integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">4</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>).</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> lines to the standard output. If the regiment <span class="tex-span"><i>i</i></span> can be made compact, the <span class="tex-span"><i>i</i></span>-th line should contain one integer, the minimal number of required moves. Otherwise, on the <span class="tex-span"><i>i</i></span>-th line print <span class="tex-font-style-tt">"-1"</span> (without quotes).</p>





```input1
4
1 1 0 0
-1 1 0 0
-1 1 0 0
1 -1 0 0
1 1 0 0
-2 1 0 0
-1 1 0 0
1 -1 0 0
1 1 0 0
-1 1 0 0
-1 1 0 0
-1 1 0 0
2 2 0 1
-1 0 0 -2
3 0 0 -2
-1 1 -2 0

```




```output1
1
-1
3
3

```



## Note

<p>In the first regiment we can move once the second or the third mole.</p><p>We can't make the second regiment compact.</p><p>In the third regiment, from the last <span class="tex-span">3</span> moles we can move once one and twice another one.</p><p>In the fourth regiment, we can move <span class="tex-font-style-bf">twice</span> the first mole and <span class="tex-font-style-bf">once</span> the third mole.</p>
