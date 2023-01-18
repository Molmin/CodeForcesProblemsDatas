## Description

<div><p>Alfred wants to buy a toy moose that costs <span class="tex-span"><i>c</i></span> dollars. The store doesn’t give change, so he must give the store exactly <span class="tex-span"><i>c</i></span> dollars, no more and no less. He has <span class="tex-span"><i>n</i></span> coins. To make <span class="tex-span"><i>c</i></span> dollars from his coins, he follows the following algorithm: let <span class="tex-span"><i>S</i></span> be the set of coins being used. <span class="tex-span"><i>S</i></span> is initially empty. Alfred repeatedly adds to <span class="tex-span"><i>S</i></span> the highest-valued coin he has such that the total value of the coins in <span class="tex-span"><i>S</i></span> after adding the coin doesn’t exceed <span class="tex-span"><i>c</i></span>. If there is no such coin, and the value of the coins in <span class="tex-span"><i>S</i></span> is still less than <span class="tex-span"><i>c</i></span>, he gives up and goes home. Note that Alfred never removes a coin from <span class="tex-span"><i>S</i></span> after adding it.</p><p>As a programmer, you might be aware that Alfred’s algorithm can fail even when there is a set of coins with value exactly <span class="tex-span"><i>c</i></span>. For example, if Alfred has one coin worth $3, one coin worth $4, and two coins worth $5, and the moose costs $12, then Alfred will add both of the $5 coins to <span class="tex-span"><i>S</i></span> and then give up, since adding any other coin would cause the value of the coins in <span class="tex-span"><i>S</i></span> to exceed $12. Of course, Alfred could instead combine one $3 coin, one $4 coin, and one $5 coin to reach the total.</p><p>Bob tried to convince Alfred that his algorithm was flawed, but Alfred didn’t believe him. Now Bob wants to give Alfred some coins (in addition to those that Alfred already has) such that Alfred’s algorithm fails. Bob can give Alfred any number of coins of any denomination (subject to the constraint that each coin must be worth a positive integer number of dollars). There can be multiple coins of a single denomination. He would like to minimize the total value of the coins he gives Alfred. Please find this minimum value. If there is no solution, print "<span class="tex-font-style-tt">Greed is good</span>". You can assume that the answer, if it exists, is positive. In other words, Alfred's algorithm will work if Bob doesn't give him any coins.</p></div><div class="input-specification"><p>The first line contains <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>c</i> ≤ 200 000</span>)&nbsp;— the price Alfred wants to pay. The second line contains <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of coins Alfred initially has. Then <span class="tex-span"><i>n</i></span> lines follow, each containing a single integer <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>c</i></span>) representing the value of one of Alfred's coins.</p></div><div class="output-specification"><p>If there is a solution, print the minimum possible total value of the coins in a solution. Otherwise, print "<span class="tex-font-style-tt">Greed is good</span>" (without quotes).</p></div>

## Input

<p>The first line contains <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>c</i> ≤ 200 000</span>)&nbsp;— the price Alfred wants to pay. The second line contains <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of coins Alfred initially has. Then <span class="tex-span"><i>n</i></span> lines follow, each containing a single integer <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>c</i></span>) representing the value of one of Alfred's coins.</p>

## Output

<p>If there is a solution, print the minimum possible total value of the coins in a solution. Otherwise, print "<span class="tex-font-style-tt">Greed is good</span>" (without quotes).</p>





```input1
12
3
5
3
4

```




```input2
50
8
1
2
4
8
16
37
37
37

```




```output1
5

```




```output2
Greed is good

```



## Note

<p>In the first sample, Bob should give Alfred a single coin worth $5. This creates the situation described in the problem statement.</p><p>In the second sample, there is no set of coins that will cause Alfred's algorithm to fail.</p>
