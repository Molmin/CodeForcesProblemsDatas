## Description

<div><p><span class="tex-font-style-it">This problem is given in two versions that differ only by constraints. If you can solve this problem in large constraints, then you can just write a single solution to the both versions. If you find the problem too difficult in large constraints, you can write solution to the simplified version only.</span></p><p>Waking up in the morning, Apollinaria decided to bake cookies. To bake one cookie, she needs <span class="tex-span"><i>n</i></span> ingredients, and for each ingredient she knows the value <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— how many grams of this ingredient one needs to bake a cookie. To prepare one cookie Apollinaria needs to use all <span class="tex-span"><i>n</i></span> ingredients.</p><p>Apollinaria has <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> gram of the <span class="tex-span"><i>i</i></span>-th ingredient. Also she has <span class="tex-span"><i>k</i></span> grams of a magic powder. Each gram of magic powder can be turned to exactly <span class="tex-span">1</span> gram of any of the <span class="tex-span"><i>n</i></span> ingredients and can be used for baking cookies.</p><p>Your task is to determine the maximum number of cookies, which Apollinaria is able to bake using the ingredients that she has and the magic powder.</p></div><div class="input-specification"><p>The first line of the input contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 1000</span>)&nbsp;— the number of ingredients and the number of grams of the magic powder.</p><p>The second line contains the sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>), where the <span class="tex-span"><i>i</i></span>-th number is equal to the number of grams of the <span class="tex-span"><i>i</i></span>-th ingredient, needed to bake one cookie.</p><p>The third line contains the sequence <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>), where the <span class="tex-span"><i>i</i></span>-th number is equal to the number of grams of the <span class="tex-span"><i>i</i></span>-th ingredient, which Apollinaria has.</p></div><div class="output-specification"><p>Print the maximum number of cookies, which Apollinaria will be able to bake using the ingredients that she has and the magic powder.</p></div>

## Input

<p>The first line of the input contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 1000</span>)&nbsp;— the number of ingredients and the number of grams of the magic powder.</p><p>The second line contains the sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>), where the <span class="tex-span"><i>i</i></span>-th number is equal to the number of grams of the <span class="tex-span"><i>i</i></span>-th ingredient, needed to bake one cookie.</p><p>The third line contains the sequence <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>), where the <span class="tex-span"><i>i</i></span>-th number is equal to the number of grams of the <span class="tex-span"><i>i</i></span>-th ingredient, which Apollinaria has.</p>

## Output

<p>Print the maximum number of cookies, which Apollinaria will be able to bake using the ingredients that she has and the magic powder.</p>





```input1
3 1
2 1 4
11 3 16

```




```input2
4 3
4 3 5 6
11 12 14 20

```




```output1
4

```




```output2
3

```



## Note

<p>In the first sample it is profitably for Apollinaria to make the existing <span class="tex-span">1</span> gram of her magic powder to ingredient with the index <span class="tex-span">2</span>, then Apollinaria will be able to bake <span class="tex-span">4</span> cookies.</p><p>In the second sample Apollinaria should turn <span class="tex-span">1</span> gram of magic powder to ingredient with the index <span class="tex-span">1</span> and <span class="tex-span">1</span> gram of magic powder to ingredient with the index <span class="tex-span">3</span>. Then Apollinaria will be able to bake <span class="tex-span">3</span> cookies. The remaining <span class="tex-span">1</span> gram of the magic powder can be left, because it can't be used to increase the answer.</p>
