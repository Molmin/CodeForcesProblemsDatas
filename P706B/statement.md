## Description

<div><p>Vasiliy likes to rest after a hard work, so you may often meet him in some bar nearby. As all programmers do, he loves the famous drink "<span class="tex-font-style-tt">Beecola</span>", which can be bought in <span class="tex-span"><i>n</i></span> different shops in the city. It's known that the price of one bottle in the shop <span class="tex-span"><i>i</i></span> is equal to <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> coins.</p><p>Vasiliy plans to buy his favorite drink for <span class="tex-span"><i>q</i></span> consecutive days. He knows, that on the <span class="tex-span"><i>i</i></span>-th day he will be able to spent <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> coins. Now, for each of the days he want to know in how many different shops he can buy a bottle of "<span class="tex-font-style-tt">Beecola</span>".</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of shops in the city that sell Vasiliy's favourite drink.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>)&nbsp;— prices of the bottles of the drink in the <span class="tex-span"><i>i</i></span>-th shop.</p><p>The third line contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 100 000</span>)&nbsp;— the number of days Vasiliy plans to buy the drink.</p><p>Then follow <span class="tex-span"><i>q</i></span> lines each containing one integer <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of coins Vasiliy can spent on the <span class="tex-span"><i>i</i></span>-th day.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>q</i></span> integers. The <span class="tex-span"><i>i</i></span>-th of them should be equal to the number of shops where Vasiliy will be able to buy a bottle of the drink on the <span class="tex-span"><i>i</i></span>-th day.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of shops in the city that sell Vasiliy's favourite drink.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>)&nbsp;— prices of the bottles of the drink in the <span class="tex-span"><i>i</i></span>-th shop.</p><p>The third line contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 100 000</span>)&nbsp;— the number of days Vasiliy plans to buy the drink.</p><p>Then follow <span class="tex-span"><i>q</i></span> lines each containing one integer <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of coins Vasiliy can spent on the <span class="tex-span"><i>i</i></span>-th day.</p>

## Output

<p>Print <span class="tex-span"><i>q</i></span> integers. The <span class="tex-span"><i>i</i></span>-th of them should be equal to the number of shops where Vasiliy will be able to buy a bottle of the drink on the <span class="tex-span"><i>i</i></span>-th day.</p>





```input1
5
3 10 8 6 11
4
1
10
3
11

```




```output1
0
4
1
5

```



## Note

<p>On the first day, Vasiliy won't be able to buy a drink in any of the shops.</p><p>On the second day, Vasiliy can buy a drink in the shops <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">3</span> and <span class="tex-span">4</span>.</p><p>On the third day, Vasiliy can buy a drink only in the shop number <span class="tex-span">1</span>.</p><p>Finally, on the last day Vasiliy can buy a drink in any shop.</p>
