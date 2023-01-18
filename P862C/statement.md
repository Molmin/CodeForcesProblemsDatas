## Description

<div><p>Mahmoud and Ehab are on the third stage of their adventures now. As you know, Dr. Evil likes sets. This time he won't show them any set from his large collection, but will ask them to create a new set to replenish his beautiful collection of sets.</p><p>Dr. Evil has his favorite evil integer <span class="tex-span"><i>x</i></span>. He asks Mahmoud and Ehab to find a set of <span class="tex-span"><i>n</i></span> distinct non-negative integers such the bitwise-xor sum of the integers in it is exactly <span class="tex-span"><i>x</i></span>. Dr. Evil doesn't like big numbers, so any number in the set shouldn't be greater than <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p></div><div class="input-specification"><p>The only line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>x</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of elements in the set and the desired bitwise-xor, respectively.</p></div><div class="output-specification"><p>If there is no such set, print "NO" (without quotes).</p><p>Otherwise, on the first line print "YES" (without quotes) and on the second line print <span class="tex-span"><i>n</i></span> distinct integers, denoting the elements in the set is any order. If there are multiple solutions you can print any of them.</p></div>

## Input

<p>The only line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>x</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of elements in the set and the desired bitwise-xor, respectively.</p>

## Output

<p>If there is no such set, print "NO" (without quotes).</p><p>Otherwise, on the first line print "YES" (without quotes) and on the second line print <span class="tex-span"><i>n</i></span> distinct integers, denoting the elements in the set is any order. If there are multiple solutions you can print any of them.</p>





```input1
5 5

```




```input2
3 6

```




```output1
YES
1 2 4 5 7
```




```output2
YES
1 2 5
```



## Note

<p>You can read more about the bitwise-xor operation here: <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">https://en.wikipedia.org/wiki/Bitwise_operation#XOR</a></p><p>For the first sample <img align="middle" class="tex-formula" src="file://DWpFIoya.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>For the second sample <img align="middle" class="tex-formula" src="file://FWFBdWqR.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
