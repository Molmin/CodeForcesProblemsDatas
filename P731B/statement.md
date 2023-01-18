## Description

<div><p>The programming competition season has already started and it's time to train for ICPC. Sereja coaches his teams for a number of year and he knows that to get ready for the training session it's not enough to prepare only problems and editorial. As the training sessions lasts for several hours, teams become hungry. Thus, Sereja orders a number of pizzas so they can eat right after the end of the competition.</p><p>Teams plan to train for <span class="tex-span"><i>n</i></span> times during <span class="tex-span"><i>n</i></span> consecutive days. During the training session Sereja orders exactly one pizza for each team that is present this day. He already knows that there will be <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> teams on the <span class="tex-span"><i>i</i></span>-th day.</p><p>There are two types of discounts in Sereja's favourite pizzeria. The first discount works if one buys two pizzas at one day, while the second is a coupon that allows to buy one pizza during two <span class="tex-font-style-bf">consecutive</span> days (two pizzas in total).</p><p>As Sereja orders really a lot of pizza at this place, he is the golden client and can use the unlimited number of discounts and coupons of any type at any days.</p><p>Sereja wants to order exactly <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> pizzas on the <span class="tex-span"><i>i</i></span>-th day while using only discounts and coupons. Note, that he will never buy more pizzas than he need for this particular day. Help him determine, whether he can buy the proper amount of pizzas each day if he is allowed to use only coupons and discounts. Note, that it's also prohibited to have any active coupons after the end of the day <span class="tex-span"><i>n</i></span>.</p></div><div class="input-specification"><p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of training sessions.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10 000</span>)&nbsp;— the number of teams that will be present on each of the days.</p></div><div class="output-specification"><p>If there is a way to order pizzas using only coupons and discounts and do not buy any extra pizzas on any of the days, then print "<span class="tex-font-style-tt">YES</span>" (without quotes) in the only line of output. Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p></div>

## Input

<p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of training sessions.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10 000</span>)&nbsp;— the number of teams that will be present on each of the days.</p>

## Output

<p>If there is a way to order pizzas using only coupons and discounts and do not buy any extra pizzas on any of the days, then print "<span class="tex-font-style-tt">YES</span>" (without quotes) in the only line of output. Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p>





```input1
4
1 2 1 2

```




```input2
3
1 0 1

```




```output1
YES

```




```output2
NO

```



## Note

<p>In the first sample, Sereja can use one coupon to buy one pizza on the first and the second days, one coupon to buy pizza on the second and the third days and one discount to buy pizzas on the fourth days. This is the only way to order pizzas for this sample.</p><p>In the second sample, Sereja can't use neither the coupon nor the discount without ordering an extra pizza. Note, that it's possible that there will be no teams attending the training sessions on some days.</p>
