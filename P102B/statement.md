## Description

<div><p>Having watched the last Harry Potter film, little Gerald also decided to practice magic. He found in his father's magical book a spell that turns any number in the sum of its digits. At the moment Gerald learned that, he came across a number <span class="tex-span"><i>n</i></span>. How many times can Gerald put a spell on it until the number becomes one-digit?</p></div><div class="input-specification"><p>The first line contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 10<sup class="upper-index">100000</sup></span>). It is guaranteed that <span class="tex-span"><i>n</i></span> doesn't contain any leading zeroes.</p></div><div class="output-specification"><p>Print the number of times a number can be replaced by the sum of its digits until it only contains one digit.</p></div>

## Input

<p>The first line contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 10<sup class="upper-index">100000</sup></span>). It is guaranteed that <span class="tex-span"><i>n</i></span> doesn't contain any leading zeroes.</p>

## Output

<p>Print the number of times a number can be replaced by the sum of its digits until it only contains one digit.</p>





```input1
0

```




```input2
10

```




```input3
991

```




```output1
0

```




```output2
1

```




```output3
3

```



## Note

<p>In the first sample the number already is one-digit — Herald can't cast a spell.</p><p>The second test contains number <span class="tex-span">10</span>. After one casting of a spell it becomes <span class="tex-span">1</span>, and here the process is completed. Thus, Gerald can only cast the spell once.</p><p>The third test contains number <span class="tex-span">991</span>. As one casts a spell the following transformations take place: <span class="tex-span">991 → 19 → 10 → 1</span>. After three transformations the number becomes one-digit.</p>
