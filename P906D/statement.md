## Description

<div><p>Priests of the Quetzalcoatl cult want to build a tower to represent a power of their god. Tower is usually made of power-charged rocks. It is built with the help of rare magic by levitating the current top of tower and adding rocks at its bottom. If top, which is built from <span class="tex-span"><i>k</i> - 1</span> rocks, possesses power <span class="tex-span"><i>p</i></span> and we want to add the rock charged with power <span class="tex-span"><i>w</i><sub class="lower-index"><i>k</i></sub></span> then value of power of a new tower will be <span class="tex-span">{<i>w</i><sub class="lower-index"><i>k</i></sub>}<sup class="upper-index"><i>p</i></sup></span>. </p><p>Rocks are added from the last to the first. That is for sequence <span class="tex-span"><i>w</i><sub class="lower-index">1</sub>, ..., <i>w</i><sub class="lower-index"><i>m</i></sub></span> value of power will be</p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://RYfWD4o0.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>After tower is built, its power may be extremely large. But still priests want to get some information about it, namely they want to know a number called cumulative power which is the true value of power taken modulo <span class="tex-span"><i>m</i></span>. Priests have <span class="tex-span"><i>n</i></span> rocks numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. They ask you to calculate which value of cumulative power will the tower possess if they will build it from rocks numbered <span class="tex-span"><i>l</i>, <i>l</i> + 1, ..., <i>r</i></span>. </p></div><div class="input-specification"><p>First line of input contains two integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>Second line of input contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>w</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>k</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) which is the power of rocks that priests have.</p><p>Third line of input contains single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) which is amount of queries from priests to you.</p><p><span class="tex-span"><i>k</i><sup class="upper-index"><i>th</i></sup></span> of next <span class="tex-span"><i>q</i></span> lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>k</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>k</i></sub> ≤ <i>r</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i></span>). </p></div><div class="output-specification"><p>Output <span class="tex-span"><i>q</i></span> integers. <span class="tex-span"><i>k</i></span>-th of them must be the amount of cumulative power the tower will have if is built from rocks <span class="tex-span"><i>l</i><sub class="lower-index"><i>k</i></sub>, <i>l</i><sub class="lower-index"><i>k</i></sub> + 1, ..., <i>r</i><sub class="lower-index"><i>k</i></sub></span>.</p></div>

## Input

<p>First line of input contains two integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>Second line of input contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>w</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>k</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) which is the power of rocks that priests have.</p><p>Third line of input contains single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) which is amount of queries from priests to you.</p><p><span class="tex-span"><i>k</i><sup class="upper-index"><i>th</i></sup></span> of next <span class="tex-span"><i>q</i></span> lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>k</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>k</i></sub> ≤ <i>r</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i></span>). </p>

## Output

<p>Output <span class="tex-span"><i>q</i></span> integers. <span class="tex-span"><i>k</i></span>-th of them must be the amount of cumulative power the tower will have if is built from rocks <span class="tex-span"><i>l</i><sub class="lower-index"><i>k</i></sub>, <i>l</i><sub class="lower-index"><i>k</i></sub> + 1, ..., <i>r</i><sub class="lower-index"><i>k</i></sub></span>.</p>





```input1
6 1000000000
1 2 2 3 3 3
8
1 1
1 6
2 2
2 3
2 4
4 4
4 5
4 6

```




```output1
1
1
2
4
256
3
27
597484987

```



## Note

<p><span class="tex-span">3<sup class="upper-index">27</sup> = 7625597484987</span></p>
