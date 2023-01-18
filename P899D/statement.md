## Description

<div><p>There are <span class="tex-span"><i>n</i></span> shovels in Polycarp's shop. The <span class="tex-span"><i>i</i></span>-th shovel costs <span class="tex-span"><i>i</i></span> burles, that is, the first shovel costs <span class="tex-span">1</span> burle, the second shovel costs <span class="tex-span">2</span> burles, the third shovel costs <span class="tex-span">3</span> burles, and so on. Polycarps wants to sell shovels in pairs.</p><p>Visitors are more likely to buy a pair of shovels if their total cost ends with several <span class="tex-span">9</span>s. Because of this, Polycarp wants to choose a pair of shovels to sell in such a way that the sum of their costs ends with maximum possible number of nines. For example, if he chooses shovels with costs <span class="tex-span">12345</span> and <span class="tex-span">37454</span>, their total cost is <span class="tex-span">49799</span>, it ends with two nines.</p><p>You are to compute the number of pairs of shovels such that their total cost ends with maximum possible number of nines. Two pairs are considered different if there is a shovel presented in one pair, but not in the other.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of shovels in Polycarp's shop.</p></div><div class="output-specification"><p>Print the number of pairs of shovels such that their total cost ends with maximum possible number of nines. </p><p>Note that it is possible that the largest number of 9s at the end is 0, then you should count all such ways.</p><p>It is guaranteed that for every <span class="tex-span"><i>n</i> ≤ 10<sup class="upper-index">9</sup></span> the answer doesn't exceed <span class="tex-span">2·10<sup class="upper-index">9</sup></span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of shovels in Polycarp's shop.</p>

## Output

<p>Print the number of pairs of shovels such that their total cost ends with maximum possible number of nines. </p><p>Note that it is possible that the largest number of 9s at the end is 0, then you should count all such ways.</p><p>It is guaranteed that for every <span class="tex-span"><i>n</i> ≤ 10<sup class="upper-index">9</sup></span> the answer doesn't exceed <span class="tex-span">2·10<sup class="upper-index">9</sup></span>.</p>





```input1
7

```




```input2
14

```




```input3
50

```




```output1
3

```




```output2
9

```




```output3
1

```



## Note

<p>In the first example the maximum possible number of nines at the end is one. Polycarp cah choose the following pairs of shovels for that purpose:</p><ul> <li> <span class="tex-span">2</span> and <span class="tex-span">7</span>; </li><li> <span class="tex-span">3</span> and <span class="tex-span">6</span>; </li><li> <span class="tex-span">4</span> and <span class="tex-span">5</span>. </li></ul><p>In the second example the maximum number of nines at the end of total cost of two shovels is one. The following pairs of shovels suit Polycarp:</p><ul> <li> <span class="tex-span">1</span> and <span class="tex-span">8</span>; </li><li> <span class="tex-span">2</span> and <span class="tex-span">7</span>; </li><li> <span class="tex-span">3</span> and <span class="tex-span">6</span>; </li><li> <span class="tex-span">4</span> and <span class="tex-span">5</span>; </li><li> <span class="tex-span">5</span> and <span class="tex-span">14</span>; </li><li> <span class="tex-span">6</span> and <span class="tex-span">13</span>; </li><li> <span class="tex-span">7</span> and <span class="tex-span">12</span>; </li><li> <span class="tex-span">8</span> and <span class="tex-span">11</span>; </li><li> <span class="tex-span">9</span> and <span class="tex-span">10</span>. </li></ul><p>In the third example it is necessary to choose shovels <span class="tex-span">49</span> and <span class="tex-span">50</span>, because the sum of their cost is <span class="tex-span">99</span>, that means that the total number of nines is equal to two, which is maximum possible for <span class="tex-span"><i>n</i> = 50</span>.</p>
