## Description

<div><p>A tourist wants to visit country Zeydabad for Zbazi (a local game in Zeydabad).</p><p>The country Zeydabad is a rectangular table consisting of <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns. Each cell on the country is either <span class="tex-font-style-tt">'z'</span> or <span class="tex-font-style-tt">'.'</span>.</p><p>The tourist knows this country is named Zeydabad because there are lots of ''<span class="tex-font-style-tt">Z-pattern</span>"s in the country. A ''<span class="tex-font-style-tt">Z-pattern</span>" is a square which anti-diagonal is completely filled with <span class="tex-font-style-tt">'z'</span> and its upper and lower rows are also completely filled with <span class="tex-font-style-tt">'z'</span>. All other cells of a square can be arbitrary.</p><center> <img class="tex-graphics" src="file://8KFdhCu5.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Note that a ''<span class="tex-font-style-tt">Z-pattern</span>" can consist of only one cell (see the examples).</p><p>So he wants to count the number of ''<span class="tex-font-style-tt">Z-pattern</span>"s in the country (a necessary skill for Zbazi).</p><p>Now your task is to help tourist with counting number of ''<span class="tex-font-style-tt">Z-pattern</span>"s.</p><p>As input/output can reach huge size it is recommended to use fast input/output methods: for example, prefer to use <span class="tex-font-style-tt">gets/scanf/printf</span> instead of <span class="tex-font-style-tt">getline/cin/cout</span> in C++, prefer to use <span class="tex-font-style-tt">BufferedReader/PrintWriter</span> instead of <span class="tex-font-style-tt">Scanner/System.out</span> in <span class="tex-font-style-tt">Java</span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 3000</span>) — the number of rows and columns respectively.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters <span class="tex-font-style-tt">'z'</span> or <span class="tex-font-style-tt">'.'</span> — the description of Zeydabad.</p></div><div class="output-specification"><p>Print the only integer <span class="tex-span"><i>a</i></span> — the number of ''<span class="tex-font-style-tt">Z-pattern</span>"s in Zeydabad.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 3000</span>) — the number of rows and columns respectively.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters <span class="tex-font-style-tt">'z'</span> or <span class="tex-font-style-tt">'.'</span> — the description of Zeydabad.</p>

## Output

<p>Print the only integer <span class="tex-span"><i>a</i></span> — the number of ''<span class="tex-font-style-tt">Z-pattern</span>"s in Zeydabad.</p>





```input1
4 4
zzzz
zzz.
.z..
zzzz

```




```input2
1 4
z.z.

```




```input3
2 2
zz
zz

```




```output1
16

```




```output2
2

```




```output3
5

```


