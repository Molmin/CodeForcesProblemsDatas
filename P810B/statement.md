## Description

<div><p>Summer holidays! Someone is going on trips, someone is visiting grandparents, but someone is trying to get a part-time job. This summer Noora decided that she wants to earn some money, and took a job in a shop as an assistant.</p><p>Shop, where Noora is working, has a plan on the following <span class="tex-span"><i>n</i></span> days. For each day sales manager knows exactly, that in <span class="tex-span"><i>i</i></span>-th day <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> products will be put up for sale and exactly <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> clients will come to the shop that day. Also, the manager is sure, that everyone, who comes to the shop, buys exactly one product or, if there aren't any left, leaves the shop without buying anything. Moreover, due to the short shelf-life of the products, manager established the following rule: if some part of the products left on the shelves at the end of the day, that products aren't kept on the next day and are sent to the dump.</p><p>For advertising purposes manager offered to start a sell-out in the shop. He asked Noora to choose any <span class="tex-span"><i>f</i></span> days from <span class="tex-span"><i>n</i></span> next for sell-outs. On each of <span class="tex-span"><i>f</i></span> chosen days the number of products were put up for sale would be doubled. Thus, if on <span class="tex-span"><i>i</i></span>-th day shop planned to put up for sale <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> products and Noora has chosen this day for sell-out, shelves of the shop would keep <span class="tex-span">2·<i>k</i><sub class="lower-index"><i>i</i></sub></span> products. Consequently, there is an opportunity to sell two times more products on days of sell-out.</p><p>Noora's task is to choose <span class="tex-span"><i>f</i></span> days to maximize total number of sold products. She asks you to help her with such a difficult problem.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>f</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>f</i> ≤ <i>n</i>)</span> denoting the number of days in shop's plan and the number of days that Noora has to choose for sell-out.</p><p>Each line of the following <span class="tex-span"><i>n</i></span> subsequent lines contains two integers <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> denoting the number of products on the shelves of the shop on the <span class="tex-span"><i>i</i></span>-th day and the number of clients that will come to the shop on <span class="tex-span"><i>i</i></span>-th day.</p></div><div class="output-specification"><p>Print a single integer denoting the maximal number of products that shop can sell.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>f</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>f</i> ≤ <i>n</i>)</span> denoting the number of days in shop's plan and the number of days that Noora has to choose for sell-out.</p><p>Each line of the following <span class="tex-span"><i>n</i></span> subsequent lines contains two integers <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> denoting the number of products on the shelves of the shop on the <span class="tex-span"><i>i</i></span>-th day and the number of clients that will come to the shop on <span class="tex-span"><i>i</i></span>-th day.</p>

## Output

<p>Print a single integer denoting the maximal number of products that shop can sell.</p>





```input1
4 2
2 1
3 5
2 3
1 5

```




```input2
4 1
0 2
0 3
3 5
0 6

```




```output1
10
```




```output2
5
```



## Note

<p>In the first example we can choose days with numbers <span class="tex-span">2</span> and <span class="tex-span">4</span> for sell-out. In this case new numbers of products for sale would be equal to <span class="tex-span">[2, 6, 2, 2]</span> respectively. So on the first day shop will sell <span class="tex-span">1</span> product, on the second&nbsp;— <span class="tex-span">5</span>, on the third&nbsp;— <span class="tex-span">2</span>, on the fourth&nbsp;— <span class="tex-span">2</span>. In total <span class="tex-span">1 + 5 + 2 + 2 = 10</span> product units.</p><p>In the second example it is possible to sell <span class="tex-span">5</span> products, if you choose third day for sell-out.</p>
