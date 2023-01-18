## Description

<div><p>Valera is a collector. Once he wanted to expand his collection with exactly one antique item.</p><p>Valera knows <span class="tex-span"><i>n</i></span> sellers of antiques, the <span class="tex-span"><i>i</i></span>-th of them auctioned <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> items. Currently the auction price of the <span class="tex-span"><i>j</i></span>-th object of the <span class="tex-span"><i>i</i></span>-th seller is <span class="tex-span"><i>s</i><sub class="lower-index"><i>ij</i></sub></span>. Valera gets on well with each of the <span class="tex-span"><i>n</i></span> sellers. He is perfectly sure that if he outbids the current price of one of the items in the auction (in other words, offers the seller the money that is strictly greater than the current price of the item at the auction), the seller of the object will immediately sign a contract with him.</p><p>Unfortunately, Valera has only <span class="tex-span"><i>v</i></span> units of money. Help him to determine which of the <span class="tex-span"><i>n</i></span> sellers he can make a deal with.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i>, <i>v</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 50;&nbsp;10<sup class="upper-index">4</sup> ≤ <i>v</i> ≤ 10<sup class="upper-index">6</sup>)</span> — the number of sellers and the units of money the Valera has.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow. The <span class="tex-span"><i>i</i></span>-th line first contains integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 50)</span> the number of items of the <span class="tex-span"><i>i</i></span>-th seller. Then go <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> space-separated integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i>1</sub>, <i>s</i><sub class="lower-index"><i>i</i>2</sub>, ..., <i>s</i><sub class="lower-index"><i>ik</i><sub class="lower-index"><i>i</i></sub></sub></span> <span class="tex-span">(10<sup class="upper-index">4</sup> ≤ <i>s</i><sub class="lower-index"><i>ij</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span> — the current prices of the items of the <span class="tex-span"><i>i</i></span>-th seller. </p></div><div class="output-specification"><p>In the first line, print integer <span class="tex-span"><i>p</i></span> — the number of sellers with who Valera can make a deal.</p><p>In the second line print <span class="tex-span"><i>p</i></span> space-separated integers <span class="tex-span"><i>q</i><sub class="lower-index">1</sub>, <i>q</i><sub class="lower-index">2</sub>, ..., <i>q</i><sub class="lower-index"><i>p</i></sub></span> <span class="tex-span">(1 ≤ <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the numbers of the sellers with who Valera can make a deal. Print the numbers of the sellers <span class="tex-font-style-bf">in the increasing order</span>. </p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i>, <i>v</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 50;&nbsp;10<sup class="upper-index">4</sup> ≤ <i>v</i> ≤ 10<sup class="upper-index">6</sup>)</span> — the number of sellers and the units of money the Valera has.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow. The <span class="tex-span"><i>i</i></span>-th line first contains integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 50)</span> the number of items of the <span class="tex-span"><i>i</i></span>-th seller. Then go <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> space-separated integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i>1</sub>, <i>s</i><sub class="lower-index"><i>i</i>2</sub>, ..., <i>s</i><sub class="lower-index"><i>ik</i><sub class="lower-index"><i>i</i></sub></sub></span> <span class="tex-span">(10<sup class="upper-index">4</sup> ≤ <i>s</i><sub class="lower-index"><i>ij</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span> — the current prices of the items of the <span class="tex-span"><i>i</i></span>-th seller. </p>

## Output

<p>In the first line, print integer <span class="tex-span"><i>p</i></span> — the number of sellers with who Valera can make a deal.</p><p>In the second line print <span class="tex-span"><i>p</i></span> space-separated integers <span class="tex-span"><i>q</i><sub class="lower-index">1</sub>, <i>q</i><sub class="lower-index">2</sub>, ..., <i>q</i><sub class="lower-index"><i>p</i></sub></span> <span class="tex-span">(1 ≤ <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the numbers of the sellers with who Valera can make a deal. Print the numbers of the sellers <span class="tex-font-style-bf">in the increasing order</span>. </p>





```input1
3 50000
1 40000
2 20000 60000
3 10000 70000 190000

```




```input2
3 50000
1 50000
3 100000 120000 110000
3 120000 110000 120000

```




```output1
3
1 2 3

```




```output2
0


```



## Note

<p>In the first sample Valera can bargain with each of the sellers. He can outbid the following items: a <span class="tex-span">40000</span> item from the first seller, a <span class="tex-span">20000</span> item from the second seller, and a <span class="tex-span">10000</span> item from the third seller.</p><p>In the second sample Valera can not make a deal with any of the sellers, as the prices of all items in the auction too big for him.</p>
