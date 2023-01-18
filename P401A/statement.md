## Description

<div><p>Vanya loves playing. He even has a special set of cards to play with. Each card has a single integer. The number on the card can be positive, negative and can even be equal to zero. The only limit is, the number on each card doesn't exceed <span class="tex-span"><i>x</i></span> in the absolute value.</p><p>Natasha doesn't like when Vanya spends a long time playing, so she hid all of his cards. Vanya became sad and started looking for the cards but he only found <span class="tex-span"><i>n</i></span> of them. Vanya loves the balance, so he wants the sum of all numbers on found cards equal to zero. On the other hand, he got very tired of looking for cards. Help the boy and say what is the minimum number of cards does he need to find to make the sum equal to zero?</p><p>You can assume that initially Vanya had infinitely many cards with each integer number from <span class="tex-span"> - <i>x</i></span> to <span class="tex-span"><i>x</i></span>.</p><p> </p></div><div class="input-specification"><p>The first line contains two integers: <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 1000)</span> — the number of found cards and <span class="tex-span"><i>x</i></span> <span class="tex-span">(1 ≤ <i>x</i> ≤ 1000)</span> — the maximum absolute value of the number on a card. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers — the numbers on found cards. It is guaranteed that the numbers do not exceed <span class="tex-span"><i>x</i></span> in their absolute value.</p></div><div class="output-specification"><p>Print a single number — the answer to the problem.</p></div>

## Input

<p>The first line contains two integers: <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 1000)</span> — the number of found cards and <span class="tex-span"><i>x</i></span> <span class="tex-span">(1 ≤ <i>x</i> ≤ 1000)</span> — the maximum absolute value of the number on a card. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers — the numbers on found cards. It is guaranteed that the numbers do not exceed <span class="tex-span"><i>x</i></span> in their absolute value.</p>

## Output

<p>Print a single number — the answer to the problem.</p>





```input1
3 2
-1 1 2

```




```input2
2 3
-2 -2

```




```output1
1

```




```output2
2

```



## Note

<p>In the first sample, Vanya needs to find a single card with number -2.</p><p>In the second sample, Vanya needs to find two cards with number 2. He can't find a single card with the required number as the numbers on the lost cards do not exceed 3 in their absolute value.</p>
