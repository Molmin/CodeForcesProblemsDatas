## Description

<div><p>One day Petya got a set of wooden cubes as a present from his mom. Petya immediately built a whole city from these cubes.</p><p>The base of the city is an <span class="tex-span"><i>n</i> × <i>n</i></span> square, divided into unit squares. The square's sides are parallel to the coordinate axes, the square's opposite corners have coordinates <span class="tex-span">(0, 0)</span> and <span class="tex-span">(<i>n</i>, <i>n</i>)</span>. On each of the unit squares Petya built a tower of wooden cubes. The side of a wooden cube also has a unit length.</p><p>After that Petya went an infinitely large distance away from his masterpiece and looked at it in the direction of vector <span class="tex-span"><i>v</i> = (<i>v</i><sub class="lower-index"><i>x</i></sub>, <i>v</i><sub class="lower-index"><i>y</i></sub>, 0)</span>. Petya wonders, how many distinct cubes are visible from this position. Help him, find this number.</p><p>Each cube includes the border. We think that a cube is visible if there is a ray emanating from some point <span class="tex-span"><i>p</i></span>, belonging to the cube, in the direction of vector <span class="tex-span"> - <i>v</i></span>, that doesn't contain any points, belonging to other cubes.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>x</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>y</i></sub></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup></span>, <span class="tex-span">|<i>v</i><sub class="lower-index"><i>x</i></sub>|, |<i>v</i><sub class="lower-index"><i>y</i></sub>| ≤ |10<sup class="upper-index">4</sup>|</span>, <span class="tex-span">|<i>v</i><sub class="lower-index"><i>x</i></sub>| + |<i>v</i><sub class="lower-index"><i>y</i></sub>| &gt; 0</span>).</p><p>Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>n</i></span> integers each: the <span class="tex-span"><i>j</i></span>-th integer in the <span class="tex-span"><i>i</i></span>-th line <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i>)</span> represents the height of the cube tower that stands on the unit square with opposite corners at points <span class="tex-span">(<i>i</i> - 1, <i>j</i> - 1)</span> and <span class="tex-span">(<i>i</i>, <i>j</i>)</span>.</p></div><div class="output-specification"><p>Print a single integer — the number of visible cubes.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>x</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>y</i></sub></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup></span>, <span class="tex-span">|<i>v</i><sub class="lower-index"><i>x</i></sub>|, |<i>v</i><sub class="lower-index"><i>y</i></sub>| ≤ |10<sup class="upper-index">4</sup>|</span>, <span class="tex-span">|<i>v</i><sub class="lower-index"><i>x</i></sub>| + |<i>v</i><sub class="lower-index"><i>y</i></sub>| &gt; 0</span>).</p><p>Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>n</i></span> integers each: the <span class="tex-span"><i>j</i></span>-th integer in the <span class="tex-span"><i>i</i></span>-th line <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i>)</span> represents the height of the cube tower that stands on the unit square with opposite corners at points <span class="tex-span">(<i>i</i> - 1, <i>j</i> - 1)</span> and <span class="tex-span">(<i>i</i>, <i>j</i>)</span>.</p>

## Output

<p>Print a single integer — the number of visible cubes.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
5 -1 2
5 0 0 0 1
0 0 0 0 2
0 0 0 1 2
0 0 0 0 2
2 2 2 2 3

```




```input2
5 1 -2
5 0 0 0 1
0 0 0 0 2
0 0 0 1 2
0 0 0 0 2
2 2 2 2 3

```




```output1
20
```




```output2
15
```


