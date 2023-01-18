## Description

<div><p>There are $n$ seats in the train's car and there is exactly one passenger occupying every seat. The seats are numbered from $1$ to $n$ from left to right. The trip is long, so each passenger will become hungry at some moment of time and will go to take boiled water for his noodles. The person at seat $i$ ($1 \leq i \leq n$) will decide to go for boiled water at minute $t_i$.</p><p>Tank with a boiled water is located to the left of the $1$-st seat. In case too many passengers will go for boiled water simultaneously, they will form a queue, since there can be only one passenger using the tank at each particular moment of time. Each passenger uses the tank for exactly $p$ minutes. We assume that the time it takes passengers to go from their seat to the tank is negligibly small. </p><p>Nobody likes to stand in a queue. So when the passenger occupying the $i$-th seat wants to go for a boiled water, he will first take a look on all seats from $1$ to $i - 1$. In case at least one of those seats is empty, he assumes that those people are standing in a queue right now, so he would be better seating for the time being. However, at the very first moment he observes that all seats with numbers smaller than $i$ are busy, he will go to the tank.</p><p>There is an unspoken rule, that in case at some moment several people can go to the tank, than only the leftmost of them (that is, seating on the seat with smallest number) will go to the tank, while all others will wait for the next moment.</p><p>Your goal is to find for each passenger, when he will receive the boiled water for his noodles.</p></div><div class="input-specification"><p>The first line contains integers $n$ and $p$ ($1 \leq n \leq 100\,000$, $1 \leq p \leq 10^9$)&nbsp;— the number of people and the amount of time one person uses the tank.</p><p>The second line contains $n$ integers $t_1, t_2, \dots, t_n$ ($0 \leq t_i \leq 10^9$)&nbsp;— the moments when the corresponding passenger will go for the boiled water.</p></div><div class="output-specification"><p>Print $n$ integers, where $i$-th of them is the time moment the passenger on $i$-th seat will receive his boiled water.</p></div>

## Input

<p>The first line contains integers $n$ and $p$ ($1 \leq n \leq 100\,000$, $1 \leq p \leq 10^9$)&nbsp;— the number of people and the amount of time one person uses the tank.</p><p>The second line contains $n$ integers $t_1, t_2, \dots, t_n$ ($0 \leq t_i \leq 10^9$)&nbsp;— the moments when the corresponding passenger will go for the boiled water.</p>

## Output

<p>Print $n$ integers, where $i$-th of them is the time moment the passenger on $i$-th seat will receive his boiled water.</p>





```input1
5 314
0 310 942 628 0
```




```output1
314 628 1256 942 1570
```



## Note

<p>Consider the example.</p><p>At the $0$-th minute there were two passengers willing to go for a water, passenger $1$ and $5$, so the first passenger has gone first, and returned at the $314$-th minute. At this moment the passenger $2$ was already willing to go for the water, so the passenger $2$ has gone next, and so on. In the end, $5$-th passenger was last to receive the boiled water.</p>
