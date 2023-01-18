## Description

<div><p>Carl is a beginner magician. He has <span class="tex-span"><i>a</i></span> blue, <span class="tex-span"><i>b</i></span> violet and <span class="tex-span"><i>c</i></span> orange magic spheres. In one move he can transform two spheres <span class="tex-font-style-bf">of the same color</span> into one sphere of any other color. To make a spell that has never been seen before, he needs at least <span class="tex-span"><i>x</i></span> blue, <span class="tex-span"><i>y</i></span> violet and <span class="tex-span"><i>z</i></span> orange spheres. Can he get them (possible, in multiple actions)?</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">0 ≤ <i>a</i>, <i>b</i>, <i>c</i> ≤ 1 000 000</span>)&nbsp;— the number of blue, violet and orange spheres that are in the magician's disposal.</p><p>The second line of the input contains three integers, <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>z</i></span> (<span class="tex-span">0 ≤ <i>x</i>, <i>y</i>, <i>z</i> ≤ 1 000 000</span>)&nbsp;— the number of blue, violet and orange spheres that he needs to get.</p></div><div class="output-specification"><p>If the wizard is able to obtain the required numbers of spheres, print "<span class="tex-font-style-tt">Yes</span>". Otherwise, print "<span class="tex-font-style-tt">No</span>".</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">0 ≤ <i>a</i>, <i>b</i>, <i>c</i> ≤ 1 000 000</span>)&nbsp;— the number of blue, violet and orange spheres that are in the magician's disposal.</p><p>The second line of the input contains three integers, <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>z</i></span> (<span class="tex-span">0 ≤ <i>x</i>, <i>y</i>, <i>z</i> ≤ 1 000 000</span>)&nbsp;— the number of blue, violet and orange spheres that he needs to get.</p>

## Output

<p>If the wizard is able to obtain the required numbers of spheres, print "<span class="tex-font-style-tt">Yes</span>". Otherwise, print "<span class="tex-font-style-tt">No</span>".</p>





```input1
4 4 0
2 1 2

```




```input2
5 6 1
2 7 2

```




```input3
3 3 3
2 2 2

```




```output1
Yes

```




```output2
No

```




```output3
Yes

```



## Note

<p>In the first sample the wizard has <span class="tex-span">4</span> blue and <span class="tex-span">4</span> violet spheres. In his first action he can turn two blue spheres into one violet one. After that he will have <span class="tex-span">2</span> blue and <span class="tex-span">5</span> violet spheres. Then he turns <span class="tex-span">4</span> violet spheres into <span class="tex-span">2</span> orange spheres and he ends up with <span class="tex-span">2</span> blue, <span class="tex-span">1</span> violet and <span class="tex-span">2</span> orange spheres, which is exactly what he needs.</p>
