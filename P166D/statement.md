## Description

<div><p>The warehouse in your shop has <span class="tex-span"><i>n</i></span> shoe pairs. Each pair is characterized by two integers: its price <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and its size <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>. We know that on this very day all numbers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> are different, that is, there is no more than one pair of each size.</p><p>The shop has <span class="tex-span"><i>m</i></span> customers who came at the same time. The customer number <span class="tex-span"><i>i</i></span> has <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> money and the size of his feet equals <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>. The customer number <span class="tex-span"><i>i</i></span> can buy the pair number <span class="tex-span"><i>j</i></span>, if <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub> ≤ <i>d</i><sub class="lower-index"><i>i</i></sub></span>, and also if <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> = <i>s</i><sub class="lower-index"><i>j</i></sub></span> or <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> = <i>s</i><sub class="lower-index"><i>j</i></sub> - 1</span>; that is, it is necessary that he has enough money to pay for the shoes. It is also necessary that the size of his feet equals to or is less by <span class="tex-span">1</span> than the size of the shoes he chooses.</p><p>Your task is to sell some customers pairs of shoes (a pair per person) so as to maximize the sum of the sold pairs <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub></span> that is, the profit. It is guaranteed that each customer buys no more than one pair and each pair will be bought by no more than one customer.</p></div><div class="input-specification"><p>The first input line contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of shoe pairs in the warehouse. Then <span class="tex-span"><i>n</i></span> lines contain the descriptions of pairs of shoes as two integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), the numbers are separated by a space. It is guaranteed that all numbers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> are different.</p><p>The next line contains an integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of customers in the shop. Next <span class="tex-span"><i>m</i></span> lines contain the customers' descriptions as two integers <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), the numbers are separated by a space.</p></div><div class="output-specification"><p>In the first line print the only integer — the maximum profit you can get from selling shoes. In the second line print an integer <span class="tex-span"><i>k</i></span> — the number of shoe pairs you will sell. In the following <span class="tex-span"><i>k</i></span> lines print the descriptions of the sold pairs — two space-separated integers where the first number is the customer's number and the second number is the number of the shoes the customer will buy.</p><p>You can print pairs of numbers "the customer's number and the shoes' number" in any order, the customers and the pairs of shoes are numbered starting from <span class="tex-span">1</span> in the order in which they are given in the input. If there are several optimal answers, you are allowed to print any of them.</p><p>Please do not use the %lld specificator to read or write 64-bit numbers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the %I64d specificator instead.</p></div>

## Input

<p>The first input line contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of shoe pairs in the warehouse. Then <span class="tex-span"><i>n</i></span> lines contain the descriptions of pairs of shoes as two integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), the numbers are separated by a space. It is guaranteed that all numbers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> are different.</p><p>The next line contains an integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of customers in the shop. Next <span class="tex-span"><i>m</i></span> lines contain the customers' descriptions as two integers <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), the numbers are separated by a space.</p>

## Output

<p>In the first line print the only integer — the maximum profit you can get from selling shoes. In the second line print an integer <span class="tex-span"><i>k</i></span> — the number of shoe pairs you will sell. In the following <span class="tex-span"><i>k</i></span> lines print the descriptions of the sold pairs — two space-separated integers where the first number is the customer's number and the second number is the number of the shoes the customer will buy.</p><p>You can print pairs of numbers "the customer's number and the shoes' number" in any order, the customers and the pairs of shoes are numbered starting from <span class="tex-span">1</span> in the order in which they are given in the input. If there are several optimal answers, you are allowed to print any of them.</p><p>Please do not use the %lld specificator to read or write 64-bit numbers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the %I64d specificator instead.</p>





```input1
3
10 1
30 2
20 3
2
20 1
20 2

```




```input2
3
10 4
20 5
30 6
2
70 4
50 5

```




```output1
30
2
2 3
1 1

```




```output2
50
2
2 3
1 2

```


