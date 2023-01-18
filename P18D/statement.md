## Description

<div><p>Last year Bob earned by selling memory sticks. During each of <span class="tex-span"><i>n</i></span> days of his work one of the two following events took place: </p><ul> <li> A customer came to Bob and asked to sell him a <span class="tex-span">2<sup class="upper-index"><i>x</i></sup></span> MB memory stick. If Bob had such a stick, he sold it and got <span class="tex-span">2<sup class="upper-index"><i>x</i></sup></span> berllars. </li><li> Bob won some programming competition and got a <span class="tex-span">2<sup class="upper-index"><i>x</i></sup></span> MB memory stick as a prize. Bob could choose whether to present this memory stick to one of his friends, or keep it. </li></ul><p>Bob never kept more than one memory stick, as he feared to mix up their capacities, and deceive a customer unintentionally. It is also known that for each memory stick capacity there was at most one customer, who wanted to buy that memory stick. Now, knowing all the customers' demands and all the prizes won at programming competitions during the last <span class="tex-span"><i>n</i></span> days, Bob wants to know, how much money he could have earned, if he had acted optimally.</p></div><div class="input-specification"><p>The first input line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>) — amount of Bob's working days. The following <span class="tex-span"><i>n</i></span> lines contain the description of the days. Line <span class="tex-font-style-tt">sell x</span> stands for a day when a customer came to Bob to buy a <span class="tex-span">2<sup class="upper-index"><i>x</i></sup></span> MB memory stick (<span class="tex-span">0 ≤ <i>x</i> ≤ 2000</span>). It's guaranteed that for each <span class="tex-span"><i>x</i></span> there is not more than one line <span class="tex-font-style-tt">sell x</span>. Line <span class="tex-font-style-tt">win x</span> stands for a day when Bob won a <span class="tex-span">2<sup class="upper-index"><i>x</i></sup></span> MB memory stick (<span class="tex-span">0 ≤ <i>x</i> ≤ 2000</span>).</p></div><div class="output-specification"><p>Output the maximum possible earnings for Bob in berllars, that he would have had if he had known all the events beforehand. Don't forget, please, that Bob can't keep more than one memory stick at a time.</p></div>

## Input

<p>The first input line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>) — amount of Bob's working days. The following <span class="tex-span"><i>n</i></span> lines contain the description of the days. Line <span class="tex-font-style-tt">sell x</span> stands for a day when a customer came to Bob to buy a <span class="tex-span">2<sup class="upper-index"><i>x</i></sup></span> MB memory stick (<span class="tex-span">0 ≤ <i>x</i> ≤ 2000</span>). It's guaranteed that for each <span class="tex-span"><i>x</i></span> there is not more than one line <span class="tex-font-style-tt">sell x</span>. Line <span class="tex-font-style-tt">win x</span> stands for a day when Bob won a <span class="tex-span">2<sup class="upper-index"><i>x</i></sup></span> MB memory stick (<span class="tex-span">0 ≤ <i>x</i> ≤ 2000</span>).</p>

## Output

<p>Output the maximum possible earnings for Bob in berllars, that he would have had if he had known all the events beforehand. Don't forget, please, that Bob can't keep more than one memory stick at a time.</p>





```input1
7
win 10
win 5
win 3
sell 5
sell 3
win 10
sell 10

```




```input2
3
win 5
sell 6
sell 4

```




```output1
1056

```




```output2
0

```


