## Description

<div><p>Little Vasya went to the supermarket to get some groceries. He walked about the supermarket for a long time and got a basket full of products. Now he needs to choose the cashier to pay for the products.</p><p>There are <span class="tex-span"><i>n</i></span> cashiers at the exit from the supermarket. At the moment the queue for the <span class="tex-span"><i>i</i></span>-th cashier already has <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> people. The <span class="tex-span"><i>j</i></span>-th person standing in the queue to the <span class="tex-span"><i>i</i></span>-th cashier has <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> items in the basket. Vasya knows that:</p><ul> <li> the cashier needs 5 seconds to scan one item; </li><li> after the cashier scans each item of some customer, he needs 15 seconds to take the customer's money and give him the change. </li></ul><p>Of course, Vasya wants to select a queue so that he can leave the supermarket as soon as possible. Help him write a program that displays the minimum number of seconds after which Vasya can get to one of the cashiers.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of cashes in the shop. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers: <span class="tex-span"><i>k</i><sub class="lower-index">1</sub>, <i>k</i><sub class="lower-index">2</sub>, ..., <i>k</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), where <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> is the number of people in the queue to the <span class="tex-span"><i>i</i></span>-th cashier.</p><p>The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> space-separated integers: <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>m</i><sub class="lower-index"><i>i</i>, 2</sub>, ..., <i>m</i><sub class="lower-index"><i>i</i>, <i>k</i><sub class="lower-index"><i>i</i></sub></sub></span> (<span class="tex-span">1 ≤ <i>m</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ 100</span>)&nbsp;— the number of products the <span class="tex-span"><i>j</i></span>-th person in the queue for the <span class="tex-span"><i>i</i></span>-th cash has.</p></div><div class="output-specification"><p>Print a single integer — the minimum number of seconds Vasya needs to get to the cashier.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of cashes in the shop. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers: <span class="tex-span"><i>k</i><sub class="lower-index">1</sub>, <i>k</i><sub class="lower-index">2</sub>, ..., <i>k</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), where <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> is the number of people in the queue to the <span class="tex-span"><i>i</i></span>-th cashier.</p><p>The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> space-separated integers: <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>m</i><sub class="lower-index"><i>i</i>, 2</sub>, ..., <i>m</i><sub class="lower-index"><i>i</i>, <i>k</i><sub class="lower-index"><i>i</i></sub></sub></span> (<span class="tex-span">1 ≤ <i>m</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ 100</span>)&nbsp;— the number of products the <span class="tex-span"><i>j</i></span>-th person in the queue for the <span class="tex-span"><i>i</i></span>-th cash has.</p>

## Output

<p>Print a single integer — the minimum number of seconds Vasya needs to get to the cashier.</p>





```input1
1
1
1

```




```input2
4
1 4 3 2
100
1 2 2 3
1 9 1
7 8

```




```output1
20

```




```output2
100

```



## Note

<p>In the second test sample, if Vasya goes to the first queue, he gets to the cashier in <span class="tex-span">100·5 + 15 = 515</span> seconds. But if he chooses the second queue, he will need <span class="tex-span">1·5 + 2·5 + 2·5 + 3·5 + 4·15 = 100</span> seconds. He will need <span class="tex-span">1·5 + 9·5 + 1·5 + 3·15 = 100</span> seconds for the third one and <span class="tex-span">7·5 + 8·5 + 2·15 = 105</span> seconds for the fourth one. Thus, Vasya gets to the cashier quicker if he chooses the second or the third queue.</p>
