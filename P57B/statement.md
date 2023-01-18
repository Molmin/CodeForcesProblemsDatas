## Description

<div><p>Chris the Rabbit found the traces of an ancient Martian civilization. The brave astronomer managed to see through a small telescope an architecture masterpiece — "A Road to the Sun". The building stands on cubical stones of the same size. The foundation divides the entire "road" into cells, into which the cubical stones are fit tightly. Thus, to any cell of the foundation a coordinate can be assigned. To become the leader of the tribe, a Martian should build a Road to the Sun, that is to build from those cubical stones on a given foundation a stairway. The stairway should be described by the number of stones in the initial coordinate and the coordinates of the stairway's beginning and end. Each following cell in the coordinate's increasing order should contain one cubical stone more than the previous one. At that if the cell has already got stones, they do not count in this building process, the stairways were simply built on them. In other words, let us assume that a stairway is built with the initial coordinate of <span class="tex-span"><i>l</i></span>, the final coordinate of <span class="tex-span"><i>r</i></span> and the number of stones in the initial coordinate <span class="tex-span"><i>x</i></span>. That means that <span class="tex-span"><i>x</i></span> stones <span class="tex-font-style-bf">will be added</span> in the cell <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>x</i> + 1</span> stones will be added in the cell <span class="tex-span"><i>l</i> + 1</span>, ..., <span class="tex-span"><i>x</i> + <i>r</i> - <i>l</i></span> stones will be added in the cell <span class="tex-span"><i>r</i></span>.</p><p>Chris managed to find an ancient manuscript, containing the descriptions of all the stairways. Now he wants to compare the data to be sure that he has really found "A Road to the Sun". For that he chose some road cells and counted the total number of cubical stones that has been accumulated throughout the Martian history and then asked you to count using the manuscript to what the sum should ideally total.</p></div><div class="input-specification"><p>The first line contains three space-separated integers: <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>k</i> ≤ <i>min</i>(<i>n</i>, 100)</span>) which is the number of cells, the number of "Roads to the Sun" and the number of cells in the query correspondingly. Each of the following <span class="tex-span"><i>m</i></span> roads contain three space-separated integers: <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) which are the stairway's description, its beginning, end and the initial cell's height. Then follow a line, containing <span class="tex-span"><i>k</i></span> different space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. All these numbers ranging from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> are cells, the number of stones in which interests Chris.</p></div><div class="output-specification"><p>You have to print a single number on a single line which is the sum of stones in all the cells Chris is interested in.</p><p>Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preffered to use <span class="tex-font-style-tt">cin</span> (also you may use <span class="tex-font-style-tt">%I64d</span>).</p></div>

## Input

<p>The first line contains three space-separated integers: <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>k</i> ≤ <i>min</i>(<i>n</i>, 100)</span>) which is the number of cells, the number of "Roads to the Sun" and the number of cells in the query correspondingly. Each of the following <span class="tex-span"><i>m</i></span> roads contain three space-separated integers: <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) which are the stairway's description, its beginning, end and the initial cell's height. Then follow a line, containing <span class="tex-span"><i>k</i></span> different space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. All these numbers ranging from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> are cells, the number of stones in which interests Chris.</p>

## Output

<p>You have to print a single number on a single line which is the sum of stones in all the cells Chris is interested in.</p><p>Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preffered to use <span class="tex-font-style-tt">cin</span> (also you may use <span class="tex-font-style-tt">%I64d</span>).</p>





```input1
5 2 1
1 5 1
2 4 1
3

```




```input2
3 2 1
1 3 1
1 3 1
2

```




```input3
3 2 1
1 3 1
1 3 1
3

```




```output1
5

```




```output2
4

```




```output3
6

```


