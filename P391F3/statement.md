## Description

<div><p><span class="tex-font-style-it">This problem consists of three subproblems: for solving subproblem F1 you will receive 8 points, for solving subproblem F2 you will receive 15 points, and for solving subproblem F3 you will receive 10 points.</span></p><p>Manao has developed a model to predict the stock price of a company over the next <span class="tex-span"><i>n</i></span> days and wants to design a profit-maximizing trading algorithm to make use of these predictions. Unfortunately, Manao's trading account has the following restrictions: </p><ul> <li> It only allows owning either zero or one shares of stock at a time; </li><li> It only allows buying or selling a share of this stock once per day; </li><li> It allows a maximum of <span class="tex-span"><i>k</i></span> buy orders over the next <span class="tex-span"><i>n</i></span> days; </li></ul><p>For the purposes of this problem, we define a <span class="tex-font-style-underline">trade</span> to a be the act of buying one share of stock on day <span class="tex-span"><i>i</i></span>, then holding the stock until some day <span class="tex-span"><i>j</i> &gt; <i>i</i></span> at which point the share is sold. To restate the above constraints, Manao is permitted to make at most <span class="tex-span"><i>k</i></span> non-overlapping trades during the course of an <span class="tex-span"><i>n</i></span>-day trading period for which Manao's model has predictions about the stock price.</p><p>Even though these restrictions limit the amount of profit Manao can make compared to what would be achievable with an unlimited number of trades or the ability to hold more than one share at a time, Manao still has the potential to make a lot of money because Manao's model perfectly predicts the daily price of the stock. For example, using this model, Manao could wait until the price is low, then buy one share and hold until the price reaches a high value, then sell for a profit, and repeat this process up to <span class="tex-span"><i>k</i></span> times until <span class="tex-span"><i>n</i></span> days have passed.</p><p>Nevertheless, Manao is not satisfied by having a merely good trading algorithm, and wants to develop an optimal strategy for trading subject to these constraints. Help Manao achieve this goal by writing a program that will determine when to buy and sell stock to achieve the greatest possible profit during the <span class="tex-span"><i>n</i></span>-day trading period subject to the above constraints.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span>, separated by a single space, with <img align="middle" class="tex-formula" src="file://dxLz7jQE.png" style="max-width: 100.0%;max-height: 100.0%;">. The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>n</i></span> lines contains a single integer <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">12</sup></span>), where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> represents the price at which someone can either buy or sell one share of stock on day <span class="tex-span"><i>i</i></span>.</p><p><span class="tex-font-style-it">The problem consists of three subproblems. The subproblems have different constraints on the input. You will get some score for the correct submission of the subproblem. The description of the subproblems follows.</span></p><ul> <li> In subproblem F1 (8 points), <span class="tex-span"><i>n</i></span> will be between <span class="tex-span">1</span> and <span class="tex-span">3000</span>, inclusive. </li><li> In subproblem F2 (15 points), <span class="tex-span"><i>n</i></span> will be between <span class="tex-span">1</span> and <span class="tex-span">100000</span>, inclusive. </li><li> In subproblem F3 (10 points), <span class="tex-span"><i>n</i></span> will be between <span class="tex-span">1</span> and <span class="tex-span">4000000</span>, inclusive. </li></ul></div><div class="output-specification"><p>For this problem, the program will only report the amount of the optimal profit, rather than a list of trades that can achieve this profit.</p><p>Therefore, the program should print one line containing a single integer, the maximum profit Manao can achieve over the next <span class="tex-span"><i>n</i></span> days with the constraints of starting with no shares on the first day of trading, always owning either zero or one shares of stock, and buying at most <span class="tex-span"><i>k</i></span> shares over the course of the <span class="tex-span"><i>n</i></span>-day trading period.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span>, separated by a single space, with <img align="middle" class="tex-formula" src="file://dxLz7jQE.png" style="max-width: 100.0%;max-height: 100.0%;">. The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>n</i></span> lines contains a single integer <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">12</sup></span>), where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> represents the price at which someone can either buy or sell one share of stock on day <span class="tex-span"><i>i</i></span>.</p><p><span class="tex-font-style-it">The problem consists of three subproblems. The subproblems have different constraints on the input. You will get some score for the correct submission of the subproblem. The description of the subproblems follows.</span></p><ul> <li> In subproblem F1 (8 points), <span class="tex-span"><i>n</i></span> will be between <span class="tex-span">1</span> and <span class="tex-span">3000</span>, inclusive. </li><li> In subproblem F2 (15 points), <span class="tex-span"><i>n</i></span> will be between <span class="tex-span">1</span> and <span class="tex-span">100000</span>, inclusive. </li><li> In subproblem F3 (10 points), <span class="tex-span"><i>n</i></span> will be between <span class="tex-span">1</span> and <span class="tex-span">4000000</span>, inclusive. </li></ul>

## Output

<p>For this problem, the program will only report the amount of the optimal profit, rather than a list of trades that can achieve this profit.</p><p>Therefore, the program should print one line containing a single integer, the maximum profit Manao can achieve over the next <span class="tex-span"><i>n</i></span> days with the constraints of starting with no shares on the first day of trading, always owning either zero or one shares of stock, and buying at most <span class="tex-span"><i>k</i></span> shares over the course of the <span class="tex-span"><i>n</i></span>-day trading period.</p>





```input1
10 2
2
7
3
9
8
7
9
7
1
9

```




```input2
10 5
2
7
3
9
8
7
9
7
1
9

```




```output1
15

```




```output2
21

```



## Note

<p>In the first example, the best trade overall is to buy at a price of <span class="tex-span">1</span> on day 9 and sell at a price of <span class="tex-span">9</span> on day 10 and the second best trade overall is to buy at a price of <span class="tex-span">2</span> on day 1 and sell at a price of <span class="tex-span">9</span> on day 4. Since these two trades do not overlap, both can be made and the profit is the sum of the profits of the two trades. Thus the trade strategy looks like this: </p><pre class="verbatim"><br>2    | 7    | 3    | 9    | 8    | 7    | 9    | 7    | 1    | 9<br>buy  |      |      | sell |      |      |      |      | buy  | sell<br></pre><p>The total profit is then <span class="tex-span">(9 - 2) + (9 - 1) = 15</span>.</p><p>In the second example, even though Manao is allowed up to 5 trades there are only 4 profitable trades available. Making a fifth trade would cost Manao money so he only makes the following 4: </p><pre class="verbatim"><br>2    | 7    | 3    | 9    | 8    | 7    | 9    | 7    | 1    | 9<br>buy  | sell | buy  | sell |      | buy  | sell |      | buy  | sell<br></pre><p>The total profit is then <span class="tex-span">(7 - 2) + (9 - 3) + (9 - 7) + (9 - 1) = 21</span>.</p>
