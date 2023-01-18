## Description

<div><p>Oleg the bank client checks share prices every day. There are <span class="tex-span"><i>n</i></span> share prices he is interested in. Today he observed that each second exactly one of these prices decreases by <span class="tex-span"><i>k</i></span> rubles (note that each second exactly one price changes, but at different seconds different prices can change). Prices can become negative. Oleg found this process interesting, and he asked Igor the financial analyst, what is the minimum time needed for all <span class="tex-span"><i>n</i></span> prices to become equal, or it is impossible at all? Igor is busy right now, so he asked you to help Oleg. Can you answer this question?</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of share prices, and the amount of rubles some price decreases each second.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the initial prices.</p></div><div class="output-specification"><p>Print the only line containing the minimum number of seconds needed for prices to become equal, of «<span class="tex-font-style-tt">-1</span>» if it is impossible.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of share prices, and the amount of rubles some price decreases each second.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the initial prices.</p>

## Output

<p>Print the only line containing the minimum number of seconds needed for prices to become equal, of «<span class="tex-font-style-tt">-1</span>» if it is impossible.</p>





```input1
3 3
12 9 15

```




```input2
2 2
10 9

```




```input3
4 1
1 1000000000 1000000000 1000000000

```




```output1
3
```




```output2
-1
```




```output3
2999999997
```



## Note

<p>Consider the first example. </p><p>Suppose the third price decreases in the first second and become equal <span class="tex-span">12</span> rubles, then the first price decreases and becomes equal <span class="tex-span">9</span> rubles, and in the third second the third price decreases again and becomes equal <span class="tex-span">9</span> rubles. In this case all prices become equal <span class="tex-span">9</span> rubles in <span class="tex-span">3</span> seconds.</p><p>There could be other possibilities, but this minimizes the time needed for all prices to become equal. Thus the answer is <span class="tex-span">3</span>.</p><p>In the second example we can notice that parity of first and second price is different and never changes within described process. Thus prices never can become equal.</p><p>In the third example following scenario can take place: firstly, the second price drops, then the third price, and then fourth price. It happens <span class="tex-span">999999999</span> times, and, since in one second only one price can drop, the whole process takes <span class="tex-span">999999999 * 3 = 2999999997</span> seconds. We can note that this is the minimum possible time.</p>
