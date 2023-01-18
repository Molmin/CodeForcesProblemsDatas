## Description

<div><p>A student's life is fraught with complications. Some Berland University students know this only too well. Having studied for two years, they contracted strong antipathy towards the chairperson of some department. Indeed, the person in question wasn't the kindest of ladies to begin with: prone to reforming groups, banning automatic passes and other mean deeds. At last the students decided that she just can't get away with all this anymore...</p><p>The students pulled some strings on the higher levels and learned that the next University directors' meeting is going to discuss <span class="tex-span"><i>n</i></span> orders about the chairperson and accept exactly <span class="tex-span"><i>p</i></span> of them. There are two values assigned to each order: <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of the chairperson's hairs that turn grey if she obeys the order and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> — the displeasement of the directors if the order isn't obeyed. The students may make the directors pass any <span class="tex-span"><i>p</i></span> orders chosen by them. The students know that the chairperson will obey exactly <span class="tex-span"><i>k</i></span> out of these <span class="tex-span"><i>p</i></span> orders. She will pick the orders to obey in the way that minimizes first, the directors' displeasement and second, the number of hairs on her head that turn grey.</p><p>The students want to choose <span class="tex-span"><i>p</i></span> orders in the way that maximizes the number of hairs on the chairperson's head that turn grey. If there are multiple ways to accept the orders, then the students are keen on maximizing the directors' displeasement with the chairperson's actions. Help them.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>p</i> ≤ <i>n</i></span>), <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>p</i></span>) — the number of orders the directors are going to discuss, the number of orders to pass and the number of orders to be obeyed by the chairperson, correspondingly. Each of the following <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), describing the corresponding order.</p></div><div class="output-specification"><p>Print <span class="tex-font-style-bf">in an arbitrary order</span> <span class="tex-span"><i>p</i></span> distinct integers — the numbers of the orders to accept so that the students could carry out the revenge. The orders are indexed from 1 to <span class="tex-span"><i>n</i></span> in the order they occur in the input. If there are multiple solutions, you can print any of them.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>p</i> ≤ <i>n</i></span>), <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>p</i></span>) — the number of orders the directors are going to discuss, the number of orders to pass and the number of orders to be obeyed by the chairperson, correspondingly. Each of the following <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), describing the corresponding order.</p>

## Output

<p>Print <span class="tex-font-style-bf">in an arbitrary order</span> <span class="tex-span"><i>p</i></span> distinct integers — the numbers of the orders to accept so that the students could carry out the revenge. The orders are indexed from 1 to <span class="tex-span"><i>n</i></span> in the order they occur in the input. If there are multiple solutions, you can print any of them.</p>





```input1
5 3 2
5 6
5 8
1 3
4 3
4 11

```




```input2
5 3 3
10 18
18 17
10 20
20 18
20 18

```




```output1
3 1 2
```




```output2
2 4 5
```



## Note

<p>In the first sample one of optimal solutions is to pass orders 1, 2, 3. In this case the chairperson obeys orders number 1 and 2. She gets 10 new grey hairs in the head and the directors' displeasement will equal 3. Note that the same result can be achieved with order 4 instead of order 3.</p><p>In the second sample, the chairperson can obey all the orders, so the best strategy for the students is to pick the orders with the maximum sum of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> values. The chairperson gets 58 new gray hairs and the directors' displeasement will equal 0.</p>
