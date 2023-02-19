## Description

<div><p>Consider a road consisting of several rows. Each row is divided into several rectangular tiles, and all tiles in the same row are equal. The first row contains exactly one rectangular tile. Look at the picture below which shows how the tiles are arranged.</p><p>The road is constructed as follows: </p><ul> <li> the first row consists of $1$ tile; </li><li> then $a_1$ rows follow; each of these rows contains $1$ tile greater than the previous row; </li><li> then $b_1$ rows follow; each of these rows contains $1$ tile less than the previous row; </li><li> then $a_2$ rows follow; each of these rows contains $1$ tile greater than the previous row; </li><li> then $b_2$ rows follow; each of these rows contains $1$ tile less than the previous row; </li><li> ... </li><li> then $a_n$ rows follow; each of these rows contains $1$ tile greater than the previous row; </li><li> then $b_n$ rows follow; each of these rows contains $1$ tile less than the previous row. </li></ul><center> <img class="tex-graphics" src="file://qFFtGcCU.png" style="max-width: 100.0%;max-height: 100.0%;"> An example of the road with $n = 2$, $a_1 = 4$, $b_1 = 2$, $a_2 = 2$, $b_2 = 3$. Rows are arranged from left to right. </center><p>You start from the only tile in the first row and want to reach the last row (any tile of it). From your current tile, you can move to any tile in the next row which touches your current tile.</p><p>Calculate the number of different paths from the first row to the last row. Since it can be large, print it modulo $998244353$.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 1000$).</p><p>Then $n$ lines follow. The $i$-th of them contains two integers $a_i$ and $b_i$ ($1 \le a_i, b_i \le 10^5$; $|a_i - b_i| \le 5$).</p><p>Additional constraint on the input: the sequence of $a_i$ and $b_i$ never results in a row with non-positive number of tiles.</p></div><div class="output-specification"><p>Print one integer — the number of paths from the first row to the last row, taken modulo $998244353$.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 1000$).</p><p>Then $n$ lines follow. The $i$-th of them contains two integers $a_i$ and $b_i$ ($1 \le a_i, b_i \le 10^5$; $|a_i - b_i| \le 5$).</p><p>Additional constraint on the input: the sequence of $a_i$ and $b_i$ never results in a row with non-positive number of tiles.</p>

## Output

<p>Print one integer — the number of paths from the first row to the last row, taken modulo $998244353$.</p>





```input1
2
4 2
2 3
```




```input2
3
4 1
2 3
3 1
```




```input3
8
328 323
867 868
715 718
721 722
439 435
868 870
834 834
797 796
```




```output1
850
```




```output2
10150
```




```output3
759099319
```


