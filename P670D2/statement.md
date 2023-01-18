## Description

<div><p>The term of this problem is the same as the previous one, the only exception — increased restrictions.</p></div><div class="input-specification"><p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000, 1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of ingredients and the number of grams of the magic powder.</p><p>The second line contains the sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where the <span class="tex-span"><i>i</i></span>-th number is equal to the number of grams of the <span class="tex-span"><i>i</i></span>-th ingredient, needed to bake one cookie.</p><p>The third line contains the sequence <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where the <span class="tex-span"><i>i</i></span>-th number is equal to the number of grams of the <span class="tex-span"><i>i</i></span>-th ingredient, which Apollinaria has.</p></div><div class="output-specification"><p>Print the maximum number of cookies, which Apollinaria will be able to bake using the ingredients that she has and the magic powder.</p></div>

## Input

<p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000, 1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of ingredients and the number of grams of the magic powder.</p><p>The second line contains the sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where the <span class="tex-span"><i>i</i></span>-th number is equal to the number of grams of the <span class="tex-span"><i>i</i></span>-th ingredient, needed to bake one cookie.</p><p>The third line contains the sequence <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where the <span class="tex-span"><i>i</i></span>-th number is equal to the number of grams of the <span class="tex-span"><i>i</i></span>-th ingredient, which Apollinaria has.</p>

## Output

<p>Print the maximum number of cookies, which Apollinaria will be able to bake using the ingredients that she has and the magic powder.</p>





```input1
1 1000000000
1
1000000000

```




```input2
10 1
1000000000 1000000000 1000000000 1000000000 1000000000 1000000000 1000000000 1000000000 1000000000 1000000000
1 1 1 1 1 1 1 1 1 1

```




```input3
3 1
2 1 4
11 3 16

```




```input4
4 3
4 3 5 6
11 12 14 20

```




```output1
2000000000

```




```output2
0

```




```output3
4

```




```output4
3

```


