## Description

<div><p>A new pack of <span class="tex-span"><i>n</i></span> t-shirts came to a shop. Each of the t-shirts is characterized by three integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is the price of the <span class="tex-span"><i>i</i></span>-th t-shirt, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is front color of the <span class="tex-span"><i>i</i></span>-th t-shirt and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is back color of the <span class="tex-span"><i>i</i></span>-th t-shirt. All values <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> are distinct, and values <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are integers from <span class="tex-span">1</span> to <span class="tex-span">3</span>.</p><p><span class="tex-span"><i>m</i></span> buyers will come to the shop. Each of them wants to buy exactly one t-shirt. For the <span class="tex-span"><i>j</i></span>-th buyer we know his favorite color <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub></span>.</p><p>A buyer agrees to buy a t-shirt, if at least one side (front or back) is painted in his favorite color. Among all t-shirts that have colors acceptable to this buyer he will choose the cheapest one. If there are no such t-shirts, the buyer won't buy anything. Assume that the buyers come one by one, and each buyer is served only after the previous one is served.</p><p>You are to compute the prices each buyer will pay for t-shirts.</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of t-shirts.</p><p>The following line contains sequence of integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000 000</span>), where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> equals to the price of the <span class="tex-span"><i>i</i></span>-th t-shirt.</p><p>The following line contains sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 3</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equals to the front color of the <span class="tex-span"><i>i</i></span>-th t-shirt.</p><p>The following line contains sequence of integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 3</span>), where <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> equals to the back color of the <span class="tex-span"><i>i</i></span>-th t-shirt.</p><p>The next line contains single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 200 000</span>)&nbsp;— the number of buyers. </p><p>The following line contains sequence <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>j</i></sub> ≤ 3</span>), where <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub></span> equals to the favorite color of the <span class="tex-span"><i>j</i></span>-th buyer. The buyers will come to the shop in the order they are given in the input. Each buyer is served only after the previous one is served.</p><p> </p></div><div class="output-specification"><p>Print to the first line <span class="tex-span"><i>m</i></span> integers — the <span class="tex-span"><i>j</i></span>-th integer should be equal to the price of the t-shirt which the <span class="tex-span"><i>j</i></span>-th buyer will buy. If the <span class="tex-span"><i>j</i></span>-th buyer won't buy anything, print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of t-shirts.</p><p>The following line contains sequence of integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000 000</span>), where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> equals to the price of the <span class="tex-span"><i>i</i></span>-th t-shirt.</p><p>The following line contains sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 3</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equals to the front color of the <span class="tex-span"><i>i</i></span>-th t-shirt.</p><p>The following line contains sequence of integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 3</span>), where <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> equals to the back color of the <span class="tex-span"><i>i</i></span>-th t-shirt.</p><p>The next line contains single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 200 000</span>)&nbsp;— the number of buyers. </p><p>The following line contains sequence <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>j</i></sub> ≤ 3</span>), where <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub></span> equals to the favorite color of the <span class="tex-span"><i>j</i></span>-th buyer. The buyers will come to the shop in the order they are given in the input. Each buyer is served only after the previous one is served.</p><p> </p>

## Output

<p>Print to the first line <span class="tex-span"><i>m</i></span> integers — the <span class="tex-span"><i>j</i></span>-th integer should be equal to the price of the t-shirt which the <span class="tex-span"><i>j</i></span>-th buyer will buy. If the <span class="tex-span"><i>j</i></span>-th buyer won't buy anything, print <span class="tex-font-style-tt">-1</span>.</p>





```input1
5
300 200 400 500 911
1 2 1 2 3
2 1 3 2 1
6
2 3 1 2 1 1

```




```input2
2
1000000000 1
1 1
1 2
2
2 1

```




```output1
200 400 300 500 911 -1 

```




```output2
1 1000000000 

```


