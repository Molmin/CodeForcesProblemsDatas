## Description

<div><p>Drazil created a following problem about putting <span class="tex-span">1 × 2</span> tiles into an <span class="tex-span"><i>n</i> × <i>m</i></span> grid:</p><p>"There is a grid with some cells that are empty and some cells that are occupied. You should use <span class="tex-span">1 × 2</span> tiles to cover all empty cells and no two tiles should cover each other. And you should print a solution about how to do it."</p><p>But Drazil doesn't like to write special checking program for this task. His friend, Varda advised him: "how about asking contestant only to print the solution <span class="tex-font-style-it">when it exists and it is unique</span>? Otherwise contestant may print '<span class="tex-font-style-tt">Not unique</span>' ".</p><p>Drazil found that the constraints for this task may be much larger than for the original task!</p><p>Can you solve this new problem?</p><p>Note that you should print '<span class="tex-font-style-tt">Not unique</span>' either when there exists no solution or when there exists several different solutions for the original task.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2000</span>).</p><p>The following <span class="tex-span"><i>n</i></span> lines describe the grid rows. Character '<span class="tex-font-style-tt">.</span>' denotes an empty cell, and the character '<span class="tex-font-style-tt">*</span>' denotes a cell that is occupied.</p></div><div class="output-specification"><p>If there is no solution or the solution is not unique, you should print the string "<span class="tex-font-style-tt">Not unique</span>".</p><p>Otherwise you should print how to cover all empty cells with <span class="tex-span">1 × 2</span> tiles. Use characters "<span class="tex-font-style-tt">&lt;&gt;</span>" to denote horizontal tiles and characters "^v" to denote vertical tiles. Refer to the sample test for the output format example.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2000</span>).</p><p>The following <span class="tex-span"><i>n</i></span> lines describe the grid rows. Character '<span class="tex-font-style-tt">.</span>' denotes an empty cell, and the character '<span class="tex-font-style-tt">*</span>' denotes a cell that is occupied.</p>

## Output

<p>If there is no solution or the solution is not unique, you should print the string "<span class="tex-font-style-tt">Not unique</span>".</p><p>Otherwise you should print how to cover all empty cells with <span class="tex-span">1 × 2</span> tiles. Use characters "<span class="tex-font-style-tt">&lt;&gt;</span>" to denote horizontal tiles and characters "^v" to denote vertical tiles. Refer to the sample test for the output format example.</p>





```input1
3 3
...
.*.
...

```




```input2
4 4
..**
*...
*.**
....

```




```input3
2 4
*..*
....

```




```input4
1 1
.

```




```input5
1 1
*

```




```output1
Not unique

```




```output2
&lt;&gt;**
*^&lt;&gt;
*v**
&lt;&gt;&lt;&gt;

```




```output3
*&lt;&gt;*
&lt;&gt;&lt;&gt;

```




```output4
Not unique

```




```output5
*

```



## Note

<p>In the first case, there are indeed two solutions:</p><pre class="verbatim"><br>&lt;&gt;^<br>^*v<br>v&lt;&gt;<br></pre><p>and</p><pre class="verbatim"><br>^&lt;&gt;<br>v*^<br>&lt;&gt;v<br></pre><p>so the answer is "<span class="tex-font-style-tt">Not unique</span>".</p>
