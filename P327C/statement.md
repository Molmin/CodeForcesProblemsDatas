## Description

<div><p>There is a long plate <span class="tex-span"><i>s</i></span> containing <span class="tex-span"><i>n</i></span> digits. Iahub wants to delete some digits (possibly none, but he is not allowed to delete all the digits) to form his "magic number" on the plate, a number that is divisible by <span class="tex-span">5</span>. Note that, the resulting number may contain leading zeros.</p><p>Now Iahub wants to count the number of ways he can obtain magic number, modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>). Two ways are different, if the set of deleted positions in <span class="tex-span"><i>s</i></span> differs.</p><p>Look at the input part of the statement, <span class="tex-span"><i>s</i></span> is given in a special form.</p></div><div class="input-specification"><p>In the first line you're given a string <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ |<i>a</i>| ≤ 10<sup class="upper-index">5</sup></span>), containing digits only. In the second line you're given an integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>). The plate <span class="tex-span"><i>s</i></span> is formed by concatenating <span class="tex-span"><i>k</i></span> copies of <span class="tex-span"><i>a</i></span> together. That is <span class="tex-span"><i>n</i> = |<i>a</i>|·<i>k</i></span>.</p></div><div class="output-specification"><p>Print a single integer — the required number of ways modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div>

## Input

<p>In the first line you're given a string <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ |<i>a</i>| ≤ 10<sup class="upper-index">5</sup></span>), containing digits only. In the second line you're given an integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>). The plate <span class="tex-span"><i>s</i></span> is formed by concatenating <span class="tex-span"><i>k</i></span> copies of <span class="tex-span"><i>a</i></span> together. That is <span class="tex-span"><i>n</i> = |<i>a</i>|·<i>k</i></span>.</p>

## Output

<p>Print a single integer — the required number of ways modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p>





```input1
1256
1

```




```input2
13990
2

```




```input3
555
2

```




```output1
4

```




```output2
528

```




```output3
63

```



## Note

<p>In the first case, there are four possible ways to make a number that is divisible by 5: 5, 15, 25 and 125.</p><p>In the second case, remember to concatenate the copies of <span class="tex-span"><i>a</i></span>. The actual plate is 1399013990.</p><p>In the third case, except deleting all digits, any choice will do. Therefore there are <span class="tex-span">2<sup class="upper-index">6</sup> - 1 = 63</span> possible ways to delete digits.</p>
