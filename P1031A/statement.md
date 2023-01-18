## Description

<div><p>You have a plate and you want to add some gilding to it. The plate is a rectangle that we split into $w\times h$ cells. There should be $k$ gilded rings, the first one should go along the edge of the plate, the second one&nbsp;— $2$ cells away from the edge and so on. Each ring has a width of $1$ cell. Formally, the $i$-th of these rings should consist of all bordering cells on the inner rectangle of size $(w - 4(i - 1))\times(h - 4(i - 1))$.</p><center> <img class="tex-graphics" height="446px" src="file://i58r9puy.png" style="max-width: 100.0%;max-height: 100.0%;" width="567px"> <span class="tex-font-size-small">The picture corresponds to the third example.</span> </center><p>Your task is to compute the number of cells to be gilded.</p></div><div class="input-specification"><p>The only line contains three integers $w$, $h$ and $k$ ($3 \le w, h \le 100$, $1 \le k \le \left\lfloor \frac{min(n, m) + 1}{4}\right\rfloor$, where $\lfloor x \rfloor$ denotes the number $x$ rounded down) — the number of rows, columns and the number of rings, respectively.</p></div><div class="output-specification"><p>Print a single positive integer&nbsp;— the number of cells to be gilded.</p></div>

## Input

<p>The only line contains three integers $w$, $h$ and $k$ ($3 \le w, h \le 100$, $1 \le k \le \left\lfloor \frac{min(n, m) + 1}{4}\right\rfloor$, where $\lfloor x \rfloor$ denotes the number $x$ rounded down) — the number of rows, columns and the number of rings, respectively.</p>

## Output

<p>Print a single positive integer&nbsp;— the number of cells to be gilded.</p>





```input1
3 3 1

```




```input2
7 9 1

```




```input3
7 9 2

```




```output1
8

```




```output2
28

```




```output3
40

```



## Note

<p>The first example is shown on the picture below.</p><center> <img class="tex-graphics" height="178px" src="file://oj438F65.png" style="max-width: 100.0%;max-height: 100.0%;" width="178px"> </center><p>The second example is shown on the picture below.</p><center> <img class="tex-graphics" height="416px" src="file://duNzwgiQ.png" style="max-width: 100.0%;max-height: 100.0%;" width="529px"> </center><p>The third example is shown in the problem description.</p>
