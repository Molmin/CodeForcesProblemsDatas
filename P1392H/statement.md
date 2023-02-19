## Description

<div><p><span class="tex-font-style-tt">zscoder</span> has a deck of $n+m$ custom-made cards, which consists of $n$ cards labelled from $1$ to $n$ and $m$ jokers. Since <span class="tex-font-style-tt">zscoder</span> is lonely, he wants to play a game with himself using those cards. </p><p>Initially, the deck is shuffled uniformly randomly and placed on the table. <span class="tex-font-style-tt">zscoder</span> has a set $S$ which is initially empty. </p><p>Every second, <span class="tex-font-style-tt">zscoder</span> draws the top card from the deck. </p><ul> <li> If the card has a number $x$ written on it, <span class="tex-font-style-tt">zscoder</span> removes the card and adds $x$ to the set $S$. </li><li> If the card drawn is a joker, <span class="tex-font-style-tt">zscoder</span> places all the cards back into the deck and reshuffles (uniformly randomly) the $n+m$ cards to form a new deck (hence the new deck now contains all cards from $1$ to $n$ and the $m$ jokers). Then, if $S$ currently contains all the elements from $1$ to $n$, the game ends. Shuffling the deck doesn't take time at all. </li></ul><p>What is the expected number of seconds before the game ends? We can show that the answer can be written in the form $\frac{P}{Q}$ where $P, Q$ are relatively prime integers and $Q \neq 0 \bmod 998244353$. Output the value of $(P \cdot Q^{-1})$ modulo $998244353$.</p></div><div class="input-specification"><p>The only line of the input contains two integers $n$ and $m$ ($1 \le n, m \le 2 \cdot 10^{6}$).</p></div><div class="output-specification"><p>Output a single integer, the value of $(P \cdot Q^{-1})$ modulo $998244353$.</p></div>

## Input

<p>The only line of the input contains two integers $n$ and $m$ ($1 \le n, m \le 2 \cdot 10^{6}$).</p>

## Output

<p>Output a single integer, the value of $(P \cdot Q^{-1})$ modulo $998244353$.</p>





```input1
2 1
```




```input2
3 2
```




```input3
14 9
```




```output1
5
```




```output2
332748127
```




```output3
969862773
```



## Note

<p>For the first sample, it can be proven that the expected time before the game ends is $5$ seconds.</p><p>For the second sample, it can be proven that the expected time before the game ends is $\frac{28}{3}$ seconds.</p>
