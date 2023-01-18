## Description

<div><p>Peppa the Pig was walking and walked into the forest. What a strange coincidence! The forest has the shape of a rectangle, consisting of <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns. We enumerate the rows of the rectangle from top to bottom with numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, and the columns — from left to right with numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>. Let's denote the cell at the intersection of the <span class="tex-span"><i>r</i></span>-th row and the <span class="tex-span"><i>c</i></span>-th column as <span class="tex-span">(<i>r</i>, <i>c</i>)</span>.</p><p>Initially the pig stands in cell <span class="tex-span">(1, 1)</span>, and in the end she wants to be in cell <span class="tex-span">(<i>n</i>, <i>m</i>)</span>. Since the pig is in a hurry to get home, she can go from cell <span class="tex-span">(<i>r</i>, <i>c</i>)</span>, only to either cell <span class="tex-span">(<i>r</i> + 1, <i>c</i>)</span> or <span class="tex-span">(<i>r</i>, <i>c</i> + 1)</span>. She cannot leave the forest.</p><p>The forest, where the pig is, is very unusual. Some cells of the forest similar to each other, and some look very different. Peppa enjoys taking pictures and at every step she takes a picture of the cell where she is now. The path through the forest is considered to be <span class="tex-font-style-it">beautiful</span> if photographs taken on her way, can be viewed in both forward and in reverse order, showing the same sequence of photos. More formally, the line formed by the cells in order of visiting should be a <span class="tex-font-style-it">palindrome</span> (you can read a formal definition of a palindrome in the previous problem).</p><p>Count the number of beautiful paths from cell <span class="tex-span">(1, 1)</span> to cell <span class="tex-span">(<i>n</i>, <i>m</i>)</span>. Since this number can be very large, determine the remainder after dividing it by <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 500</span>) — the height and width of the field.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> lowercase English letters identifying the types of cells of the forest. Identical cells are represented by identical letters, different cells are represented by different letters.</p></div><div class="output-specification"><p>Print a single integer — the number of beautiful paths modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 500</span>) — the height and width of the field.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> lowercase English letters identifying the types of cells of the forest. Identical cells are represented by identical letters, different cells are represented by different letters.</p>

## Output

<p>Print a single integer — the number of beautiful paths modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
3 4
aaab
baaa
abba

```




```output1
3
```



## Note

<p>Picture illustrating possibilities for the sample test. </p><center> <img class="tex-graphics" src="file://bYYfNHEa.png" style="max-width: 100.0%;max-height: 100.0%;"> <p><img class="tex-graphics" src="file://0Np4kASV.png" style="max-width: 100.0%;max-height: 100.0%;"> </p><p><img class="tex-graphics" src="file://lkK8iXcg.png" style="max-width: 100.0%;max-height: 100.0%;"> </p></center>
