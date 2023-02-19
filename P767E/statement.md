## Description

<div><p>Student Arseny likes to plan his life for <span class="tex-span"><i>n</i></span> days ahead. He visits a canteen every day and he has already decided what he will order in each of the following <span class="tex-span"><i>n</i></span> days. Prices in the canteen do not change and that means Arseny will spend <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> rubles during the <span class="tex-span"><i>i</i></span>-th day.</p><p>There are <span class="tex-span">1</span>-ruble coins and <span class="tex-span">100</span>-ruble notes in circulation. At this moment, Arseny has <span class="tex-span"><i>m</i></span> coins and a sufficiently large amount of notes (you can assume that he has an infinite amount of them). Arseny loves modern technologies, so he uses his credit card everywhere except the canteen, but he has to pay in cash in the canteen because it does not accept cards.</p><p>Cashier always asks the student to pay change-free. However, it's not always possible, but Arseny tries to minimize the <span class="tex-font-style-it">dissatisfaction</span> of the cashier. Cashier's dissatisfaction for each of the days is determined by the total amount of notes and coins in the change. To be precise, if the cashier gives Arseny <span class="tex-span"><i>x</i></span> notes and coins on the <span class="tex-span"><i>i</i></span>-th day, his dissatisfaction for this day equals <span class="tex-span"><i>x</i>·<i>w</i><sub class="lower-index"><i>i</i></sub></span>. Cashier always gives change using as little coins and notes as possible, he always has enough of them to be able to do this.</p><center> <img class="tex-graphics" height="378px" src="file://E8GIo4cq.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px">   <span class="tex-font-size-small">"Caution! Angry cashier"</span> </center><p>Arseny wants to pay in such a way that the total dissatisfaction of the cashier for <span class="tex-span"><i>n</i></span> days would be as small as possible. Help him to find out how he needs to pay in each of the <span class="tex-span"><i>n</i></span> days!</p><p>Note that Arseny always has enough money to pay, because he has an infinite amount of notes. Arseny can use notes and coins he received in change during any of the following days.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the amount of days Arseny planned his actions for and the amount of coins he currently has. </p><p>The second line contains a sequence of integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the amounts of money in rubles which Arseny is going to spend for each of the following days. </p><p>The third line contains a sequence of integers <span class="tex-span"><i>w</i><sub class="lower-index">1</sub>, <i>w</i><sub class="lower-index">2</sub>, ..., <i>w</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the cashier's dissatisfaction coefficients for each of the following days.</p></div><div class="output-specification"><p>In the first line print one integer&nbsp;— minimum possible total dissatisfaction of the cashier.</p><p>Then print <span class="tex-span"><i>n</i></span> lines, the <span class="tex-span"><i>i</i></span>-th of then should contain two numbers&nbsp;— the amount of notes and the amount of coins which Arseny should use to pay in the canteen on the <span class="tex-span"><i>i</i></span>-th day.</p><p>Of course, the total amount of money Arseny gives to the casher in any of the days should be no less than the amount of money he has planned to spend. It also shouldn't exceed <span class="tex-span">10<sup class="upper-index">6</sup></span> rubles: Arseny never carries large sums of money with him.</p><p>If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the amount of days Arseny planned his actions for and the amount of coins he currently has. </p><p>The second line contains a sequence of integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the amounts of money in rubles which Arseny is going to spend for each of the following days. </p><p>The third line contains a sequence of integers <span class="tex-span"><i>w</i><sub class="lower-index">1</sub>, <i>w</i><sub class="lower-index">2</sub>, ..., <i>w</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the cashier's dissatisfaction coefficients for each of the following days.</p>

## Output

<p>In the first line print one integer&nbsp;— minimum possible total dissatisfaction of the cashier.</p><p>Then print <span class="tex-span"><i>n</i></span> lines, the <span class="tex-span"><i>i</i></span>-th of then should contain two numbers&nbsp;— the amount of notes and the amount of coins which Arseny should use to pay in the canteen on the <span class="tex-span"><i>i</i></span>-th day.</p><p>Of course, the total amount of money Arseny gives to the casher in any of the days should be no less than the amount of money he has planned to spend. It also shouldn't exceed <span class="tex-span">10<sup class="upper-index">6</sup></span> rubles: Arseny never carries large sums of money with him.</p><p>If there are multiple answers, print any of them.</p>





```input1
5 42
117 71 150 243 200
1 1 1 1 1

```




```input2
3 0
100 50 50
1 3 2

```




```input3
5 42
117 71 150 243 200
5 4 3 2 1

```




```output1
79
1 17
1 0
2 0
2 43
2 0

```




```output2
150
1 0
1 0
0 50

```




```output3
230
1 17
1 0
1 50
3 0
2 0

```


