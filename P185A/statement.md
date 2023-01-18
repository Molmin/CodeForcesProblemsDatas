## Description

<div><p>Dwarfs have planted a very interesting plant, which is a triangle directed "upwards". This plant has an amusing feature. After one year a triangle plant directed "upwards" divides into four triangle plants: three of them will point "upwards" and one will point "downwards". After another year, each triangle plant divides into four triangle plants: three of them will be directed in the same direction as the parent plant, and one of them will be directed in the opposite direction. Then each year the process repeats. The figure below illustrates this process.</p><center> <img class="tex-graphics" src="file://8oFns99Y.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Help the dwarfs find out how many triangle plants that point "upwards" will be in <span class="tex-span"><i>n</i></span> years.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(0 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup>)</span> — the number of full years when the plant grew.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div><div class="output-specification"><p>Print a single integer — the remainder of dividing the number of plants that will point "upwards" in <span class="tex-span"><i>n</i></span> years by <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(0 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup>)</span> — the number of full years when the plant grew.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>

## Output

<p>Print a single integer — the remainder of dividing the number of plants that will point "upwards" in <span class="tex-span"><i>n</i></span> years by <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
1

```




```input2
2

```




```output1
3

```




```output2
10

```



## Note

<p>The first test sample corresponds to the second triangle on the figure in the statement. The second test sample corresponds to the third one.</p>
