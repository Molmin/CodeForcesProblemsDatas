## Description

<div><p>You take part in the testing of new weapon. For the testing a polygon was created. The polygon is a rectangular field <span class="tex-span"><i>n</i> × <i>m</i></span> in size, divided into unit squares <span class="tex-span">1 × 1</span> in size. The polygon contains <span class="tex-span"><i>k</i></span> objects, each of which is a rectangle with sides, parallel to the polygon sides and entirely occupying several unit squares. The objects don't intersect and don't touch each other.</p><p>The principle according to which the weapon works is highly secret. You only know that one can use it to strike any rectangular area whose area is not equal to zero with sides, parallel to the sides of the polygon. The area must completely cover some of the unit squares into which the polygon is divided and it must not touch the other squares. Of course the area mustn't cross the polygon border. Your task is as follows: you should hit no less than one and no more than three rectangular objects. Each object must either lay completely inside the area (in that case it is considered to be hit), or lay completely outside the area.</p><p>Find the number of ways of hitting.</p></div><div class="input-specification"><p>The first line has three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> и <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 90</span>) — the sizes of the polygon and the number of objects on it respectively. Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> symbols each and describe the polygon. The symbol "<span class="tex-font-style-tt">*</span>" stands for a square occupied an object, whereas the symbol "<span class="tex-font-style-tt">.</span>" stands for an empty space. The symbols "<span class="tex-font-style-tt">*</span>" form exactly <span class="tex-span"><i>k</i></span> rectangular connected areas that meet the requirements of the task.</p></div><div class="output-specification"><p>Output a single number — the number of different ways to hit a target.</p></div>

## Input

<p>The first line has three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> и <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 90</span>) — the sizes of the polygon and the number of objects on it respectively. Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> symbols each and describe the polygon. The symbol "<span class="tex-font-style-tt">*</span>" stands for a square occupied an object, whereas the symbol "<span class="tex-font-style-tt">.</span>" stands for an empty space. The symbols "<span class="tex-font-style-tt">*</span>" form exactly <span class="tex-span"><i>k</i></span> rectangular connected areas that meet the requirements of the task.</p>

## Output

<p>Output a single number — the number of different ways to hit a target.</p>





```input1
3 3 3
*.*
...
*..

```




```input2
4 5 4
.*.**
...**
**...
...**

```




```input3
2 2 1
.*
..

```




```output1
21

```




```output2
38

```




```output3
4

```


