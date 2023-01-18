## Description

<div><p>All our characters have hobbies. The same is true for Fedor. He enjoys shopping in the neighboring supermarket. </p><p>The goods in the supermarket have unique integer ids. Also, for every integer there is a product with id equal to this integer. Fedor has <span class="tex-span"><i>n</i></span> discount coupons, the <span class="tex-span"><i>i</i></span>-th of them can be used with products with ids ranging from <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, inclusive. Today Fedor wants to take exactly <span class="tex-span"><i>k</i></span> coupons with him.</p><p>Fedor wants to choose the <span class="tex-span"><i>k</i></span> coupons in such a way that the number of such products <span class="tex-span"><i>x</i></span> that all coupons can be used with this product <span class="tex-span"><i>x</i></span> is as large as possible (for better understanding, see examples). Fedor wants to save his time as well, so he asks you to choose coupons for him. Help Fedor!</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of coupons Fedor has, and the number of coupons he wants to choose.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the description of the <span class="tex-span"><i>i</i></span>-th coupon. The coupons can be equal.</p></div><div class="output-specification"><p>In the first line print single integer&nbsp;— the maximum number of products with which all the chosen coupons can be used. The products with which at least one coupon cannot be used shouldn't be counted.</p><p>In the second line print <span class="tex-span"><i>k</i></span> distinct integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the ids of the coupons which Fedor should choose.</p><p>If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of coupons Fedor has, and the number of coupons he wants to choose.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the description of the <span class="tex-span"><i>i</i></span>-th coupon. The coupons can be equal.</p>

## Output

<p>In the first line print single integer&nbsp;— the maximum number of products with which all the chosen coupons can be used. The products with which at least one coupon cannot be used shouldn't be counted.</p><p>In the second line print <span class="tex-span"><i>k</i></span> distinct integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the ids of the coupons which Fedor should choose.</p><p>If there are multiple answers, print any of them.</p>





```input1
4 2
1 100
40 70
120 130
125 180

```




```input2
3 2
1 12
15 20
25 30

```




```input3
5 2
1 10
5 15
14 50
30 70
99 100

```




```output1
31
1 2 

```




```output2
0
1 2 

```




```output3
21
3 4 

```



## Note

<p>In the first example if we take the first two coupons then all the products with ids in range <span class="tex-span">[40, 70]</span> can be bought with both coupons. There are <span class="tex-span">31</span> products in total.</p><p>In the second example, no product can be bought with two coupons, that is why the answer is <span class="tex-span">0</span>. Fedor can choose any two coupons in this example.</p>
