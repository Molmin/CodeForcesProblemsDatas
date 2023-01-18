## Description

<div><p>The big consignment of t-shirts goes on sale in the shop before the beginning of the spring. In all <span class="tex-span"><i>n</i></span> types of t-shirts go on sale. The t-shirt of the <span class="tex-span"><i>i</i></span>-th type has two integer parameters — <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span>, where <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> — is the price of the <span class="tex-span"><i>i</i></span>-th type t-shirt, <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> — is the quality of the <span class="tex-span"><i>i</i></span>-th type t-shirt. It should be assumed that the unlimited number of t-shirts of each type goes on sale in the shop, but in general the quality is not concerned with the price. </p><p>As predicted, <span class="tex-span"><i>k</i></span> customers will come to the shop within the next month, the <span class="tex-span"><i>j</i></span>-th customer will get ready to spend up to <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> on buying t-shirts. </p><p>All customers have the same strategy. First of all, the customer wants to buy the maximum possible number of the highest quality t-shirts, then to buy the maximum possible number of the highest quality t-shirts from residuary t-shirts and so on. At the same time among several same quality t-shirts the customer will buy one that is cheaper. The customers don't like the same t-shirts, so each customer will not buy more than one t-shirt of one type. </p><p>Determine the number of t-shirts which each customer will buy, if they use the described strategy. All customers act independently from each other, and the purchase of one does not affect the purchase of another.</p></div><div class="input-specification"><p>The first line contains the positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of t-shirt types. </p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the price and the quality of the <span class="tex-span"><i>i</i></span>-th type t-shirt.</p><p>The next line contains the positive integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of the customers. </p><p>The next line contains <span class="tex-span"><i>k</i></span> positive integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where the <span class="tex-span"><i>j</i></span>-th number is equal to the sum, which the <span class="tex-span"><i>j</i></span>-th customer gets ready to spend on t-shirts.</p></div><div class="output-specification"><p>The first line of the input data should contain the sequence of <span class="tex-span"><i>k</i></span> integers, where the <span class="tex-span"><i>i</i></span>-th number should be equal to the number of t-shirts, which the <span class="tex-span"><i>i</i></span>-th customer will buy.</p></div>

## Input

<p>The first line contains the positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of t-shirt types. </p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the price and the quality of the <span class="tex-span"><i>i</i></span>-th type t-shirt.</p><p>The next line contains the positive integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of the customers. </p><p>The next line contains <span class="tex-span"><i>k</i></span> positive integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where the <span class="tex-span"><i>j</i></span>-th number is equal to the sum, which the <span class="tex-span"><i>j</i></span>-th customer gets ready to spend on t-shirts.</p>

## Output

<p>The first line of the input data should contain the sequence of <span class="tex-span"><i>k</i></span> integers, where the <span class="tex-span"><i>i</i></span>-th number should be equal to the number of t-shirts, which the <span class="tex-span"><i>i</i></span>-th customer will buy.</p>





```input1
3
7 5
3 5
4 3
2
13 14

```




```input2
2
100 500
50 499
4
50 200 150 100

```




```output1
2 3 

```




```output2
1 2 2 1 

```



## Note

<p>In the first example the first customer will buy the t-shirt of the second type, then the t-shirt of the first type. He will spend 10 and will not be able to buy the t-shirt of the third type because it costs 4, and the customer will owe only 3. The second customer will buy all three t-shirts (at first, the t-shirt of the second type, then the t-shirt of the first type, and then the t-shirt of the third type). He will spend all money on it. </p>
