## Description

<div><p>Andrew was very excited to participate in Olympiad of Metropolises. Days flew by quickly, and Andrew is already at the airport, ready to go home. He has $n$ rubles left, and would like to exchange them to euro and dollar bills. Andrew can mix dollar bills and euro bills in whatever way he wants. The price of one dollar is $d$ rubles, and one euro costs $e$ rubles.</p><p>Recall that there exist the following dollar bills: $1$, $2$, $5$, $10$, $20$, $50$, $100$, and the following euro bills&nbsp;— $5$, $10$, $20$, $50$, $100$, $200$ (note that, in this problem we do <span class="tex-font-style-bf">not</span> consider the $500$ euro bill, it is hard to find such bills in the currency exchange points). Andrew can buy any combination of bills, and his goal is to minimize the total number of rubles he will have after the exchange.</p><p>Help him&nbsp;— write a program that given integers $n$, $e$ and $d$, finds the minimum number of rubles Andrew can get after buying dollar and euro bills.</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($1 \leq n \leq 10^8$)&nbsp;— the initial sum in rubles Andrew has. </p><p>The second line of the input contains one integer $d$ ($30 \leq d \leq 100$)&nbsp;— the price of one dollar in rubles. </p><p>The third line of the input contains integer $e$ ($30 \leq e \leq 100$)&nbsp;— the price of one euro in rubles.</p></div><div class="output-specification"><p>Output one integer&nbsp;— the minimum number of rubles Andrew can have after buying dollar and euro bills optimally.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($1 \leq n \leq 10^8$)&nbsp;— the initial sum in rubles Andrew has. </p><p>The second line of the input contains one integer $d$ ($30 \leq d \leq 100$)&nbsp;— the price of one dollar in rubles. </p><p>The third line of the input contains integer $e$ ($30 \leq e \leq 100$)&nbsp;— the price of one euro in rubles.</p>

## Output

<p>Output one integer&nbsp;— the minimum number of rubles Andrew can have after buying dollar and euro bills optimally.</p>





```input1
100
60
70
```




```input2
410
55
70
```




```input3
600
60
70
```




```output1
40
```




```output2
5
```




```output3
0
```



## Note

<p>In the first example, we can buy just $1$ dollar because there is no $1$ euro bill.</p><p>In the second example, optimal exchange is to buy $5$ euro and $1$ dollar.</p><p>In the third example, optimal exchange is to buy $10$ dollars in one bill.</p>
