## Description

<div><p>Anton's favourite geometric figures are regular polyhedrons. Note that there are five kinds of regular polyhedrons: </p><ul> <li> <span class="tex-font-style-it">Tetrahedron</span>. Tetrahedron has <span class="tex-span">4</span> triangular faces. </li><li> <span class="tex-font-style-it">Cube</span>. Cube has <span class="tex-span">6</span> square faces. </li><li> <span class="tex-font-style-it">Octahedron</span>. Octahedron has <span class="tex-span">8</span> triangular faces. </li><li> <span class="tex-font-style-it">Dodecahedron</span>. Dodecahedron has <span class="tex-span">12</span> pentagonal faces. </li><li> <span class="tex-font-style-it">Icosahedron</span>. Icosahedron has <span class="tex-span">20</span> triangular faces. </li></ul><p>All five kinds of polyhedrons are shown on the picture below:</p><center> <img class="tex-graphics" src="file://Qizlomey.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Anton has a collection of <span class="tex-span"><i>n</i></span> polyhedrons. One day he decided to know, how many faces his polyhedrons have in total. Help Anton and find this number!</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 200 000)</span>&nbsp;— the number of polyhedrons in Anton's collection.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines of the input contains a string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— the name of the <span class="tex-span"><i>i</i></span>-th polyhedron in Anton's collection. The string can look like this:</p><ul> <li> "<span class="tex-font-style-tt">Tetrahedron</span>" (without quotes), if the <span class="tex-span"><i>i</i></span>-th polyhedron in Anton's collection is a tetrahedron. </li><li> "<span class="tex-font-style-tt">Cube</span>" (without quotes), if the <span class="tex-span"><i>i</i></span>-th polyhedron in Anton's collection is a cube. </li><li> "<span class="tex-font-style-tt">Octahedron</span>" (without quotes), if the <span class="tex-span"><i>i</i></span>-th polyhedron in Anton's collection is an octahedron. </li><li> "<span class="tex-font-style-tt">Dodecahedron</span>" (without quotes), if the <span class="tex-span"><i>i</i></span>-th polyhedron in Anton's collection is a dodecahedron. </li><li> "<span class="tex-font-style-tt">Icosahedron</span>" (without quotes), if the <span class="tex-span"><i>i</i></span>-th polyhedron in Anton's collection is an icosahedron. </li></ul></div><div class="output-specification"><p>Output one number&nbsp;— the total number of faces in all the polyhedrons in Anton's collection.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 200 000)</span>&nbsp;— the number of polyhedrons in Anton's collection.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines of the input contains a string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— the name of the <span class="tex-span"><i>i</i></span>-th polyhedron in Anton's collection. The string can look like this:</p><ul> <li> "<span class="tex-font-style-tt">Tetrahedron</span>" (without quotes), if the <span class="tex-span"><i>i</i></span>-th polyhedron in Anton's collection is a tetrahedron. </li><li> "<span class="tex-font-style-tt">Cube</span>" (without quotes), if the <span class="tex-span"><i>i</i></span>-th polyhedron in Anton's collection is a cube. </li><li> "<span class="tex-font-style-tt">Octahedron</span>" (without quotes), if the <span class="tex-span"><i>i</i></span>-th polyhedron in Anton's collection is an octahedron. </li><li> "<span class="tex-font-style-tt">Dodecahedron</span>" (without quotes), if the <span class="tex-span"><i>i</i></span>-th polyhedron in Anton's collection is a dodecahedron. </li><li> "<span class="tex-font-style-tt">Icosahedron</span>" (without quotes), if the <span class="tex-span"><i>i</i></span>-th polyhedron in Anton's collection is an icosahedron. </li></ul>

## Output

<p>Output one number&nbsp;— the total number of faces in all the polyhedrons in Anton's collection.</p>





```input1
4
Icosahedron
Cube
Tetrahedron
Dodecahedron

```




```input2
3
Dodecahedron
Octahedron
Octahedron

```




```output1
42

```




```output2
28

```



## Note

<p>In the first sample Anton has one icosahedron, one cube, one tetrahedron and one dodecahedron. Icosahedron has <span class="tex-span">20</span> faces, cube has <span class="tex-span">6</span> faces, tetrahedron has <span class="tex-span">4</span> faces and dodecahedron has <span class="tex-span">12</span> faces. In total, they have <span class="tex-span">20 + 6 + 4 + 12 = 42</span> faces.</p>
