## Description

<div><p>Ayush is a cashier at the shopping center. Recently his department has started a ''<span class="tex-font-style-tt">click and collect</span>" service which allows users to shop online. </p><p>The store contains <span class="tex-span"><i>k</i></span> items. <span class="tex-span"><i>n</i></span> customers have already used the above service. Each user paid for <span class="tex-span"><i>m</i></span> items. Let <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> denote the <span class="tex-span"><i>j</i></span>-th item in the <span class="tex-span"><i>i</i></span>-th person's order.</p><p>Due to the space limitations all the items are arranged in one single row. When Ayush receives the <span class="tex-span"><i>i</i></span>-th order he will find one by one all the items <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>m</i></span>) in the row. Let <span class="tex-span"><i>pos</i>(<i>x</i>)</span> denote the position of the item <span class="tex-span"><i>x</i></span> in the row at the moment of its collection. Then Ayush takes time equal to <span class="tex-span"><i>pos</i>(<i>a</i><sub class="lower-index"><i>i</i>1</sub>) + <i>pos</i>(<i>a</i><sub class="lower-index"><i>i</i>2</sub>) + ... + <i>pos</i>(<i>a</i><sub class="lower-index"><i>im</i></sub>)</span> for the <span class="tex-span"><i>i</i></span>-th customer.</p><p>When Ayush accesses the <span class="tex-span"><i>x</i></span>-th element he keeps a new stock in the front of the row and takes away the <span class="tex-span"><i>x</i></span>-th element. Thus the values are updating.</p><p>Your task is to calculate the total time it takes for Ayush to process all the orders.</p><p>You can assume that the market has endless stock.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 100, 1 ≤ <i>m</i> ≤ <i>k</i></span>) — the number of users, the number of items each user wants to buy and the total number of items at the market.</p><p>The next line contains <span class="tex-span"><i>k</i></span> distinct integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>l</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>l</i></sub> ≤ <i>k</i></span>) denoting the initial positions of the items in the store. The items are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i></span>.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ <i>k</i></span>) — the order of the <span class="tex-span"><i>i</i></span>-th person.</p></div><div class="output-specification"><p>Print the only integer <span class="tex-span"><i>t</i></span> — the total time needed for Ayush to process all the orders.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 100, 1 ≤ <i>m</i> ≤ <i>k</i></span>) — the number of users, the number of items each user wants to buy and the total number of items at the market.</p><p>The next line contains <span class="tex-span"><i>k</i></span> distinct integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>l</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>l</i></sub> ≤ <i>k</i></span>) denoting the initial positions of the items in the store. The items are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i></span>.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ <i>k</i></span>) — the order of the <span class="tex-span"><i>i</i></span>-th person.</p>

## Output

<p>Print the only integer <span class="tex-span"><i>t</i></span> — the total time needed for Ayush to process all the orders.</p>





```input1
2 2 5
3 4 1 2 5
1 5
3 1

```




```output1
14

```



## Note

<p>Customer <span class="tex-span">1</span> wants the items <span class="tex-span">1</span> and <span class="tex-span">5</span>.</p><p><span class="tex-span"><i>pos</i>(1) = 3</span>, so the new positions are: <span class="tex-span">[1, 3, 4, 2, 5]</span>.</p><p><span class="tex-span"><i>pos</i>(5) = 5</span>, so the new positions are: <span class="tex-span">[5, 1, 3, 4, 2]</span>.</p><p>Time taken for the first customer is <span class="tex-span">3 + 5 = 8</span>.</p><p>Customer <span class="tex-span">2</span> wants the items <span class="tex-span">3</span> and <span class="tex-span">1</span>.</p><p><span class="tex-span"><i>pos</i>(3) = 3</span>, so the new positions are: <span class="tex-span">[3, 5, 1, 4, 2]</span>.</p><p><span class="tex-span"><i>pos</i>(1) = 3</span>, so the new positions are: <span class="tex-span">[1, 3, 5, 4, 2]</span>.</p><p>Time taken for the second customer is <span class="tex-span">3 + 3 = 6</span>.</p><p>Total time is <span class="tex-span">8 + 6 = 14</span>.</p><p>Formally <span class="tex-span"><i>pos</i>(<i>x</i>)</span> is the index of <span class="tex-span"><i>x</i></span> in the current row.</p>
