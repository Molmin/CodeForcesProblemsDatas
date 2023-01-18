## Description

<div><p>Nothing has changed since the last round. Dima and Inna still love each other and want to be together. They've made a deal with Seryozha and now they need to make a deal with the dorm guards...</p><p>There are four guardposts in Dima's dorm. Each post contains two guards (in Russia they are usually elderly women). You can bribe a guard by a chocolate bar or a box of juice. For each guard you know the minimum price of the chocolate bar she can accept as a gift and the minimum price of the box of juice she can accept as a gift. If a chocolate bar for some guard costs less than the minimum chocolate bar price for this guard is, or if a box of juice for some guard costs less than the minimum box of juice price for this guard is, then the guard doesn't accept such a gift.</p><p>In order to pass through a guardpost, one needs to bribe both guards.</p><p>The shop has an unlimited amount of juice and chocolate of any price starting with <span class="tex-span">1</span>. Dima wants to choose some guardpost, buy one gift for each guard from the guardpost and spend <span class="tex-font-style-bf">exactly</span> <span class="tex-span"><i>n</i></span> rubles on it.</p><p>Help him choose a post through which he can safely sneak Inna or otherwise say that this is impossible. Mind you, Inna would be very sorry to hear that!</p></div><div class="input-specification"><p>The first line of the input contains integer <span class="tex-span"><i>n</i>&nbsp;(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the money Dima wants to spend. Then follow four lines describing the guardposts. Each line contains four integers <span class="tex-span"><i>a</i>, <i>b</i>, <i>c</i>, <i>d</i>&nbsp;(1 ≤ <i>a</i>, <i>b</i>, <i>c</i>, <i>d</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the minimum price of the chocolate and the minimum price of the juice for the first guard and the minimum price of the chocolate and the minimum price of the juice for the second guard, correspondingly.</p></div><div class="output-specification"><p>In a single line of the output print three space-separated integers: the number of the guardpost, the cost of the first present and the cost of the second present. If there is no guardpost Dima can sneak Inna through at such conditions, print -1 in a single line. </p><p>The guardposts are numbered from <span class="tex-span">1</span> to <span class="tex-span">4</span> according to the order given in the input.</p><p>If there are multiple solutions, you can print any of them.</p></div>

## Input

<p>The first line of the input contains integer <span class="tex-span"><i>n</i>&nbsp;(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the money Dima wants to spend. Then follow four lines describing the guardposts. Each line contains four integers <span class="tex-span"><i>a</i>, <i>b</i>, <i>c</i>, <i>d</i>&nbsp;(1 ≤ <i>a</i>, <i>b</i>, <i>c</i>, <i>d</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the minimum price of the chocolate and the minimum price of the juice for the first guard and the minimum price of the chocolate and the minimum price of the juice for the second guard, correspondingly.</p>

## Output

<p>In a single line of the output print three space-separated integers: the number of the guardpost, the cost of the first present and the cost of the second present. If there is no guardpost Dima can sneak Inna through at such conditions, print -1 in a single line. </p><p>The guardposts are numbered from <span class="tex-span">1</span> to <span class="tex-span">4</span> according to the order given in the input.</p><p>If there are multiple solutions, you can print any of them.</p>





```input1
10
5 6 5 6
6 6 7 7
5 8 6 6
9 9 9 9

```




```input2
10
6 6 6 6
7 7 7 7
4 4 4 4
8 8 8 8

```




```input3
5
3 3 3 3
3 3 3 3
3 3 3 3
3 3 3 3

```




```output1
1 5 5

```




```output2
3 4 6

```




```output3
-1

```



## Note

<p>Explanation of the first example.</p><p>The only way to spend 10 rubles to buy the gifts that won't be less than the minimum prices is to buy two 5 ruble chocolates to both guards from the first guardpost.</p><p>Explanation of the second example.</p><p>Dima needs 12 rubles for the first guardpost, 14 for the second one, 16 for the fourth one. So the only guardpost we can sneak through is the third one. So, Dima can buy 4 ruble chocolate for the first guard and 6 ruble juice of the second guard.</p>
