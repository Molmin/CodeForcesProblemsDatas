## Description

<div><p>You want to train a neural network model for your graduation work. There are $n$ images in the dataset, the $i$-th image's size is $a_i$ bytes.</p><p>You don't have any powerful remote servers to train this model so you have to do it on your local machine. But there is a problem: the total size of the dataset is too big for your machine, so you decided to remove some images — though you don't want to make the dataset too weak so you can remove <span class="tex-font-style-bf">no more than</span> $k$ images from it. Note that you can only remove images, you <span class="tex-font-style-bf">can't change their order</span>.</p><p>You want to remove these images optimally so you came up with a metric (you're a data scientist after all) that allows to measure the result of removals. Consider the array $b_1, b_2, \ldots, b_m$ after removing at most $k$ images ($n - k \le m \le n$). The data from this array will be uploaded to the machine in blocks of $x$ <span class="tex-font-style-bf">consecutive</span> elements each. More precisely:</p><ul> <li> elements with indices from $1$ to $x$ ($b_1, b_2, \ldots, b_x$) belong to the first block; </li><li> elements with indices from $x + 1$ to $2x$ ($b_{x + 1}, b_{x + 2}, \ldots, b_{2x}$) belong to the second block; </li><li> elements with indices from $2x + 1$ to $3x$ ($b_{2x + 1}, b_{2x + 2}, \ldots, b_{3x}$) belong to the third block; </li><li> and so on. </li></ul><p>There will be $cnt = \left\lceil\frac{m}{x}\right\rceil$ blocks in total. Note that if $m$ is not divisible by $x$ then the last block contains less than $x$ elements, and it's okay.</p><p>Let $w(i)$ be the total size of the $i$-th block — that is, the sum of sizes of images inside this block. For example, the size of the first block $w(1)$ is $b_1 + b_2 + \ldots + b_x$, the size of the second block $w(2)$ is $b_{x + 1} + b_{x + 2} + \ldots + b_{2x}$.</p><p>The value of the metric you came up with is the <span class="tex-font-style-bf">maximum</span> block size over the blocks of the resulting dataset. In other words, the value of the metric is $\max\limits_{i=1}^{cnt} w(i)$.</p><p>You don't want to overload your machine too much, so you have to remove at most $k$ images in a way that <span class="tex-font-style-bf">minimizes</span> the value of the metric described above.</p></div><div class="input-specification"><p>The first line of the input contains three integers $n$, $k$ and $x$ ($1 \le n \le 10^5$; $1 \le k, x \le n$) — the number of images in the dataset, the maximum number of images you can remove and the length of each block (except maybe for the last one), respectively.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^5$), where $a_i$ is the size of the $i$-th image.</p></div><div class="output-specification"><p>Print one integer: the <span class="tex-font-style-bf">minimum</span> possible value of the metric described in the problem statement after removing no more than $k$ images from the dataset.</p></div>

## Input

<p>The first line of the input contains three integers $n$, $k$ and $x$ ($1 \le n \le 10^5$; $1 \le k, x \le n$) — the number of images in the dataset, the maximum number of images you can remove and the length of each block (except maybe for the last one), respectively.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^5$), where $a_i$ is the size of the $i$-th image.</p>

## Output

<p>Print one integer: the <span class="tex-font-style-bf">minimum</span> possible value of the metric described in the problem statement after removing no more than $k$ images from the dataset.</p>





```input1
5 5 4
1 1 5 4 5
```




```input2
5 2 4
6 1 5 5 6
```




```input3
6 1 4
3 3 1 3 1 2
```




```input4
6 1 3
2 2 1 2 2 1
```




```output1
0
```




```output2
11
```




```output3
8
```




```output4
5
```



## Note

<p>In the first example, you can remove the whole array so the answer is $0$.</p><p>In the second example, you can remove the first and the last elements of $a$ and obtain $b = [1, 5, 5]$. The size of the first (and the only) block is $11$. So the answer is $11$.</p><p>In the third example, you can remove the second element of $a$ and obtain $b = [3, 1, 3, 1, 2]$. The size of the first block is $8$ and the size of the second block is $2$. So the answer is $8$.</p><p>In the fourth example, you can keep the array $a$ unchanged and obtain $b = [2, 2, 1, 2, 2, 1]$. The size of the first block is $5$ as well as the size of the second block. So the answer is $5$.</p>
