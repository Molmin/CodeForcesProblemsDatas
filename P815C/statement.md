## Description

<div><p>On the way home, Karen decided to stop by the supermarket to buy some groceries.</p><center> <img class="tex-graphics" src="file://M9TX8CTH.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>She needs to buy a lot of goods, but since she is a student her budget is still quite limited. In fact, she can only spend up to <span class="tex-span"><i>b</i></span> dollars.</p><p>The supermarket sells <span class="tex-span"><i>n</i></span> goods. The <span class="tex-span"><i>i</i></span>-th good can be bought for <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> dollars. Of course, each good can only be bought once.</p><p>Lately, the supermarket has been trying to increase its business. Karen, being a loyal customer, was given <span class="tex-span"><i>n</i></span> coupons. If Karen purchases the <span class="tex-span"><i>i</i></span>-th good, she can use the <span class="tex-span"><i>i</i></span>-th coupon to decrease its price by <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>. Of course, a coupon cannot be used without buying the corresponding good.</p><p>There is, however, a constraint with the coupons. For all <span class="tex-span"><i>i</i> ≥ 2</span>, in order to use the <span class="tex-span"><i>i</i></span>-th coupon, Karen must also use the <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>-th coupon (which may mean using even more coupons to satisfy the requirement for that coupon).</p><p>Karen wants to know the following. What is the maximum number of goods she can buy, without exceeding her budget <span class="tex-span"><i>b</i></span>?</p></div><div class="input-specification"><p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>, <span class="tex-span">1 ≤ <i>b</i> ≤ 10<sup class="upper-index">9</sup></span>), the number of goods in the store and the amount of money Karen has, respectively.</p><p>The next <span class="tex-span"><i>n</i></span> lines describe the items. Specifically:</p><ul> <li> The <span class="tex-span"><i>i</i></span>-th line among these starts with two integers, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> &lt; <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), the price of the <span class="tex-span"><i>i</i></span>-th good and the discount when using the coupon for the <span class="tex-span"><i>i</i></span>-th good, respectively. </li><li> If <span class="tex-span"><i>i</i> ≥ 2</span>, this is followed by another integer, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i></span>), denoting that the <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>-th coupon must also be used before this coupon can be used. </li></ul></div><div class="output-specification"><p>Output a single integer on a line by itself, the number of different goods Karen can buy, without exceeding her budget.</p></div>

## Input

<p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>, <span class="tex-span">1 ≤ <i>b</i> ≤ 10<sup class="upper-index">9</sup></span>), the number of goods in the store and the amount of money Karen has, respectively.</p><p>The next <span class="tex-span"><i>n</i></span> lines describe the items. Specifically:</p><ul> <li> The <span class="tex-span"><i>i</i></span>-th line among these starts with two integers, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> &lt; <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), the price of the <span class="tex-span"><i>i</i></span>-th good and the discount when using the coupon for the <span class="tex-span"><i>i</i></span>-th good, respectively. </li><li> If <span class="tex-span"><i>i</i> ≥ 2</span>, this is followed by another integer, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i></span>), denoting that the <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>-th coupon must also be used before this coupon can be used. </li></ul>

## Output

<p>Output a single integer on a line by itself, the number of different goods Karen can buy, without exceeding her budget.</p>





```input1
6 16
10 9
10 5 1
12 2 1
20 18 3
10 2 3
2 1 5

```




```input2
5 10
3 1
3 1 1
3 1 2
3 1 3
3 1 4

```




```output1
4

```




```output2
5

```



## Note

<p>In the first test case, Karen can purchase the following <span class="tex-span">4</span> items:</p><ul> <li> Use the first coupon to buy the first item for <span class="tex-span">10 - 9 = 1</span> dollar. </li><li> Use the third coupon to buy the third item for <span class="tex-span">12 - 2 = 10</span> dollars. </li><li> Use the fourth coupon to buy the fourth item for <span class="tex-span">20 - 18 = 2</span> dollars. </li><li> Buy the sixth item for <span class="tex-span">2</span> dollars. </li></ul><p>The total cost of these goods is <span class="tex-span">15</span>, which falls within her budget. Note, for example, that she cannot use the coupon on the sixth item, because then she should have also used the fifth coupon to buy the fifth item, which she did not do here.</p><p>In the second test case, Karen has enough money to use all the coupons and purchase everything.</p>
