## Description

<div><p>Gerald has been selling state secrets at leisure. All the secrets cost the same: <span class="tex-span"><i>n</i></span> marks. The state which secrets Gerald is selling, has no paper money, only coins. But there are coins of all positive integer denominations that are powers of three: 1 mark, 3 marks, 9 marks, 27 marks and so on. There are no coins of other denominations. Of course, Gerald likes it when he gets money without the change. And all buyers respect him and try to give the desired sum without change, if possible. But this does not always happen.</p><p>One day an unlucky buyer came. He did not have the desired sum without change. Then he took out all his coins and tried to give Gerald a larger than necessary sum with as few coins as possible. What is the maximum number of coins he could get?</p><p><span class="tex-font-style-it">The formal explanation of the previous paragraph:</span> we consider all the possible combinations of coins for which the buyer can not give Gerald the sum of <span class="tex-span"><i>n</i></span> marks without change. For each such combination calculate the minimum number of coins that can bring the buyer at least <span class="tex-span"><i>n</i></span> marks. Among all combinations choose the maximum of the minimum number of coins. This is the number we want.</p></div><div class="input-specification"><p>The single line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">17</sup></span>).</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64 bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div><div class="output-specification"><p>In a single line print an integer: the maximum number of coins the unlucky buyer could have paid with.</p></div>

## Input

<p>The single line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">17</sup></span>).</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64 bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>

## Output

<p>In a single line print an integer: the maximum number of coins the unlucky buyer could have paid with.</p>





```input1
1

```




```input2
4

```




```output1
1

```




```output2
2

```



## Note

<p>In the first test case, if a buyer has exactly one coin of at least 3 marks, then, to give Gerald one mark, he will have to give this coin. In this sample, the customer can not have a coin of one mark, as in this case, he will be able to give the money to Gerald without any change.</p><p>In the second test case, if the buyer had exactly three coins of 3 marks, then, to give Gerald 4 marks, he will have to give two of these coins. The buyer cannot give three coins as he wants to minimize the number of coins that he gives.</p>
