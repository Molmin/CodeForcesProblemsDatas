## Description

<div><p>As you know, majority of students and teachers of Summer Informatics School live in Berland for the most part of the year. Since corruption there is quite widespread, the following story is not uncommon.</p><p>Elections are coming. You know the number of voters and the number of parties&nbsp;— $n$ and $m$ respectively. For each voter you know the party he is going to vote for. However, he can easily change his vote given a certain amount of money. In particular, if you give $i$-th voter $c_i$ bytecoins you can ask him to vote for any other party you choose.</p><p>The United Party of Berland has decided to perform a statistical study&nbsp;— you need to calculate the minimum number of bytecoins the Party needs to spend to ensure its victory. In order for a party to win the elections, it needs to receive strictly more votes than any other party.</p></div><div class="input-specification"><p>The first line of input contains two integers $n$ and $m$ ($1 \le n, m \le 3000$)&nbsp;— the number of voters and the number of parties respectively.</p><p>Each of the following $n$ lines contains two integers $p_i$ and $c_i$ ($1 \le p_i \le m$, $1 \le c_i \le 10^9$)&nbsp;— the index of this voter's preferred party and the number of bytecoins needed for him to reconsider his decision.</p><p>The United Party of Berland has the index $1$.</p></div><div class="output-specification"><p>Print a single number&nbsp;— the minimum number of bytecoins needed for The United Party of Berland to win the elections.</p></div>

## Input

<p>The first line of input contains two integers $n$ and $m$ ($1 \le n, m \le 3000$)&nbsp;— the number of voters and the number of parties respectively.</p><p>Each of the following $n$ lines contains two integers $p_i$ and $c_i$ ($1 \le p_i \le m$, $1 \le c_i \le 10^9$)&nbsp;— the index of this voter's preferred party and the number of bytecoins needed for him to reconsider his decision.</p><p>The United Party of Berland has the index $1$.</p>

## Output

<p>Print a single number&nbsp;— the minimum number of bytecoins needed for The United Party of Berland to win the elections.</p>





```input1
1 2
1 100

```




```input2
5 5
2 100
3 200
4 300
5 400
5 900

```




```input3
5 5
2 100
3 200
4 300
5 800
5 900

```




```output1
0

```




```output2
500

```




```output3
600

```



## Note

<p>In the first sample, The United Party wins the elections even without buying extra votes.</p><p>In the second sample, The United Party can buy the votes of the first and the fourth voter. This way The Party gets two votes, while parties $3$, $4$ and $5$ get one vote and party number $2$ gets no votes.</p><p>In the third sample, The United Party can buy the votes of the first three voters and win, getting three votes against two votes of the fifth party.</p>
