## Description

<div><p>One day Polycarpus stopped by a supermarket on his way home. It turns out that the supermarket is having a special offer for stools. The offer is as follows: if a customer's shopping cart contains at least one stool, the customer gets a <span class="tex-span">50%</span> discount on the cheapest item in the cart (that is, it becomes two times cheaper). If there are several items with the same minimum price, the discount is available for only one of them!</p><p>Polycarpus has <span class="tex-span"><i>k</i></span> carts, and he wants to buy up all stools and pencils from the supermarket. Help him distribute the stools and the pencils among the shopping carts, so that the items' total price (including the discounts) is the least possible.</p><p>Polycarpus must use all <span class="tex-span"><i>k</i></span> carts to purchase the items, no shopping cart can remain empty. Each shopping cart can contain an arbitrary number of stools and/or pencils.</p></div><div class="input-specification"><p>The first input line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup></span>) — the number of items in the supermarket and the number of carts, correspondingly. Next <span class="tex-span"><i>n</i></span> lines describe the items as "<span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>" (without the quotes), where <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) is an integer denoting the price of the <span class="tex-span"><i>i</i></span>-th item, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>) is an integer representing the type of item <span class="tex-span"><i>i</i></span> (<span class="tex-span">1</span> for a stool and <span class="tex-span">2</span> for a pencil). The numbers in the lines are separated by single spaces.</p></div><div class="output-specification"><p>In the first line print a single real number <span class="tex-font-style-bf">with exactly one </span> decimal place — the minimum total price of the items, including the discounts.</p><p>In the following <span class="tex-span"><i>k</i></span> lines print the descriptions of the items in the carts. In the <span class="tex-span"><i>i</i></span>-th line print the description of the <span class="tex-span"><i>i</i></span>-th cart as "<span class="tex-span"><i>t</i></span> <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>b</i><sub class="lower-index">2</sub></span> <span class="tex-span">...</span> <span class="tex-span"><i>b</i><sub class="lower-index"><i>t</i></sub></span>" (without the quotes), where <span class="tex-span"><i>t</i></span> is the number of items in the <span class="tex-span"><i>i</i></span>-th cart, and the sequence <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>t</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>) gives the indices of items to put in this cart in the optimal distribution. All indices of items in all carts should be pairwise different, each item must belong to exactly one cart. You can print the items in carts and the carts themselves in any order. The items are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in the order in which they are specified in the input.</p><p>If there are multiple optimal distributions, you are allowed to print any of them.</p></div>

## Input

<p>The first input line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup></span>) — the number of items in the supermarket and the number of carts, correspondingly. Next <span class="tex-span"><i>n</i></span> lines describe the items as "<span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>" (without the quotes), where <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) is an integer denoting the price of the <span class="tex-span"><i>i</i></span>-th item, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>) is an integer representing the type of item <span class="tex-span"><i>i</i></span> (<span class="tex-span">1</span> for a stool and <span class="tex-span">2</span> for a pencil). The numbers in the lines are separated by single spaces.</p>

## Output

<p>In the first line print a single real number <span class="tex-font-style-bf">with exactly one </span> decimal place — the minimum total price of the items, including the discounts.</p><p>In the following <span class="tex-span"><i>k</i></span> lines print the descriptions of the items in the carts. In the <span class="tex-span"><i>i</i></span>-th line print the description of the <span class="tex-span"><i>i</i></span>-th cart as "<span class="tex-span"><i>t</i></span> <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>b</i><sub class="lower-index">2</sub></span> <span class="tex-span">...</span> <span class="tex-span"><i>b</i><sub class="lower-index"><i>t</i></sub></span>" (without the quotes), where <span class="tex-span"><i>t</i></span> is the number of items in the <span class="tex-span"><i>i</i></span>-th cart, and the sequence <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>t</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>) gives the indices of items to put in this cart in the optimal distribution. All indices of items in all carts should be pairwise different, each item must belong to exactly one cart. You can print the items in carts and the carts themselves in any order. The items are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in the order in which they are specified in the input.</p><p>If there are multiple optimal distributions, you are allowed to print any of them.</p>





```input1
3 2
2 1
3 2
3 1

```




```input2
4 3
4 1
1 2
2 2
3 2

```




```output1
5.5
2 1 2
1 3

```




```output2
8.0
1 1
2 4 2
1 3

```



## Note

<p>In the first sample case the first cart should contain the 1st and 2nd items, and the second cart should contain the 3rd item. This way each cart has a stool and each cart has a <span class="tex-span">50%</span> discount for the cheapest item. The total price of all items will be: <span class="tex-span">2·0.5 + (3 + 3·0.5) = 1 + 4.5 = 5.5</span>.</p>
