## Description

<div><p>After the fourth season Sherlock and Moriary have realized the whole foolishness of the battle between them and decided to continue their competitions in peaceful game of Credit Cards.</p><p>Rules of this game are simple: each player bring his favourite <span class="tex-span"><i>n</i></span>-digit credit card. Then both players name the digits written on their cards one by one. If two digits are not equal, then the player, whose digit is smaller gets a flick (knock in the forehead usually made with a forefinger) from the other player. For example, if <span class="tex-span"><i>n</i> = 3</span>, Sherlock's card is <span class="tex-span">123</span> and Moriarty's card has number <span class="tex-span">321</span>, first Sherlock names <span class="tex-span">1</span> and Moriarty names <span class="tex-span">3</span> so Sherlock gets a flick. Then they both digit <span class="tex-span">2</span> so no one gets a flick. Finally, Sherlock names <span class="tex-span">3</span>, while Moriarty names <span class="tex-span">1</span> and gets a flick.</p><p>Of course, Sherlock will play honestly naming digits one by one in the order they are given, while Moriary, as a true villain, plans to cheat. He is going to name his digits in some other order (however, he is not going to change the overall number of occurences of each digit). For example, in case above Moriarty could name <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">3</span> and get no flicks at all, or he can name <span class="tex-span">2</span>, <span class="tex-span">3</span> and <span class="tex-span">1</span> to give Sherlock two flicks.</p><p>Your goal is to find out the minimum possible number of flicks Moriarty will get (no one likes flicks) and the maximum possible number of flicks Sherlock can get from Moriarty. Note, that these two goals are different and the optimal result may be obtained by using different strategies.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the number of digits in the cards Sherlock and Moriarty are going to use.</p><p>The second line contains <span class="tex-span"><i>n</i></span> digits&nbsp;— Sherlock's credit card number.</p><p>The third line contains <span class="tex-span"><i>n</i></span> digits&nbsp;— Moriarty's credit card number.</p></div><div class="output-specification"><p>First print the minimum possible number of flicks Moriarty will get. Then print the maximum possible number of flicks that Sherlock can get from Moriarty.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the number of digits in the cards Sherlock and Moriarty are going to use.</p><p>The second line contains <span class="tex-span"><i>n</i></span> digits&nbsp;— Sherlock's credit card number.</p><p>The third line contains <span class="tex-span"><i>n</i></span> digits&nbsp;— Moriarty's credit card number.</p>

## Output

<p>First print the minimum possible number of flicks Moriarty will get. Then print the maximum possible number of flicks that Sherlock can get from Moriarty.</p>





```input1
3
123
321

```




```input2
2
88
00

```




```output1
0
2

```




```output2
2
0

```



## Note

<p>First sample is elaborated in the problem statement. In the second sample, there is no way Moriarty can avoid getting two flicks.</p>
