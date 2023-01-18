## Description

<div><p>Michael has just bought a new electric car for moving across city. Michael does not like to overwork, so each day he drives to only one of two his jobs.</p><p>Michael's day starts from charging his electric car for getting to the work and back. He spends <span class="tex-span">1000</span> burles on charge if he goes to the first job, and <span class="tex-span">2000</span> burles if he goes to the second job.</p><p>On a charging station he uses there is a loyalty program that involves bonus cards. Bonus card may have some non-negative amount of bonus burles. Each time customer is going to buy something for the price of <span class="tex-span"><i>x</i></span> burles, he is allowed to pay an amount of <span class="tex-span"><i>y</i></span> (<span class="tex-span">0 ≤ <i>y</i> ≤ <i>x</i></span>) burles that does not exceed the bonus card balance with bonus burles. In this case he pays <span class="tex-span"><i>x</i> - <i>y</i></span> burles with cash, and the balance on the bonus card is decreased by <span class="tex-span"><i>y</i></span> bonus burles. </p><p>If customer pays whole price with cash (i.e., <span class="tex-span"><i>y</i> = 0</span>) then 10% of price is returned back to the bonus card. This means that bonus card balance increases by <img align="middle" class="tex-formula" src="file://zugT3P02.png" style="max-width: 100.0%;max-height: 100.0%;"> bonus burles. Initially the bonus card balance is equal to 0 bonus burles.</p><p>Michael has planned next <span class="tex-span"><i>n</i></span> days and he knows how much does the charge cost on each of those days. Help Michael determine the minimum amount of burles in cash he has to spend with optimal use of bonus card. Assume that Michael is able to cover any part of the price with cash in any day. It is not necessary to spend all bonus burles at the end of the given period.</p></div><div class="input-specification"><p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300 000</span>), the number of days Michael has planned.</p><p>Next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 1000</span> or <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 2000</span>) with <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> denoting the charging cost at the day <span class="tex-span"><i>i</i></span>.</p></div><div class="output-specification"><p>Output the minimum amount of burles Michael has to spend.</p></div>

## Input

<p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300 000</span>), the number of days Michael has planned.</p><p>Next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 1000</span> or <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 2000</span>) with <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> denoting the charging cost at the day <span class="tex-span"><i>i</i></span>.</p>

## Output

<p>Output the minimum amount of burles Michael has to spend.</p>





```input1
3
1000 2000 1000

```




```input2
6
2000 2000 2000 2000 2000 1000

```




```output1
3700

```




```output2
10000

```



## Note

<p>In the first sample case the most optimal way for Michael is to pay for the first two days spending 3000 burles and get 300 bonus burles as return. After that he is able to pay only 700 burles for the third days, covering the rest of the price with bonus burles.</p><p>In the second sample case the most optimal way for Michael is to pay the whole price for the first five days, getting 1000 bonus burles as return and being able to use them on the last day without paying anything in cash.</p>
